# Martín's Sprint 3 Business Question

**Question:** How often do users add a product manually?

This is **Type 3**, related to feature usage: it shows how much manual entry is used compared with saving recommendations, helping the team decide which saving flow to improve. The metric measures the share of currently saved products, rather than historical action frequency.

## Data contract

- The metric uses the existing shared Firestore collections, `products` and `productEvents`. It does not introduce a new collection.
- Classification follows the existing rules in `functions/analytics/core_saving_features.py`, also used by the core saving features metric.
- Products whose document IDs do not start with `rec_` are classified as manually added.
- A recommended product must match a `recommendation_shown` event with a valid `savedAt`, `userId`, `sourceProductId` and `savedProductId`. The saved product ID must match `rec_<SHA256(userId:sourceProductId)>`, and the product's `ownerId` must match the event's user.
- Products starting with `rec_` without a matching valid event are reported as unclassified. Duplicate recommendation events do not count the same product more than once.

## Calculation

The `manual_product_usage` metric of `get_admin_analytics` (`functions/analytics/manual_product_usage.py` in the backend) reads current products and product events:

- `manualProducts` is the number of products classified as manually added;
- `recommendedProducts` is the number linked to a confirmed recommendation save;
- `classifiedProducts` is the sum of those two counts;
- **`manualPercentage`** is `manualProducts / classifiedProducts × 100`, rounded to one decimal place;
- `unclassifiedProducts` reports products excluded from the percentage, and `totalCurrentProducts` includes all current products;
- when there are no classified products, the percentage is unavailable rather than 0%.

The Admin Web shows the result in the **Manual product usage** view (`src/manual-product-usage-view.js`). It displays the percentage, manual and recommended counts, unclassified products, and the calculation's scope. Refresh requests updated counts from the backend.

## Interpretation and limits

- This is the composition of currently saved products, not the number of save actions over time. Deleting a product removes it from the calculation.
- “Manual” follows the existing product ID convention. The metric does not separately identify manual, link and voice entry. A product containing a URL is not automatically classified as an add-by-link action.
- Unclassified products are excluded from the percentage and shown separately so missing classification is visible.
- The result counts products, not unique users. Users who save more products contribute more records.

## Evidence

Backend: 6 tests in `tests/test_manual_product_usage.py`, covering empty data, manual and recommended counts, duplicate recommendation events, unclassified products, deleted products, shared Firestore collection reads, and endpoint registration and admin access. The backend suite passed all 147 tests during validation.

Admin Web: 2 tests in `test/manual-product-usage-view.test.js`, covering the displayed backend percentage and the empty state. The dashboard suite passed all 33 tests, and the production build succeeded during validation.

The backend deployment and dashboard verification were completed.

<!-- Upload your dashboard screenshot, then replace the path below with its actual path. -->

<img src="evidence/manual_product_usage_admin_web.png" width="760" alt="Admin Web Manual product usage view">

<!-- Replace the placeholders below with your actual PR numbers and URLs. -->

Related work: backend [PR #NUMBER](BACKEND_PR_URL) and Admin Web [PR #NUMBER](DASHBOARD_PR_URL).
