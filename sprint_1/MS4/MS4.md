# MS4 – Integrating Analytics

Team: #13

Members: Juliana Duran 202220671, Santiago Casasbuenas 202214932, Martin Riveira 202321727, Jeronimo Franco 202222204, Juan Felipe Saenz 202311148, Miguel Angel Velandia 202312487.

---

## 1. Problem & Solution Description

> Write two short descriptions: one for the problem selected and one for the proposed solution.

**Problem:** *(To be completed by the team — short description of the selected problem, consistent with the one carried forward from MS2/MS3.)*

**Solution:** *(To be completed by the team — short description of the proposed solution, consistent with MS3 §5.)*

---

## 2. Analytics Persona

> Submit **one extra persona** for the problem. An analytics persona is different from a prospective user (the personas submitted in MS3) — it represents someone inside the product/business who would use the app's *data* to make decisions (e.g., a product manager, growth lead, or founder), not someone who uses the app itself. Use the template provided by the course (Chapter 3 of the book).

| # | Analytics Persona | Description | Source (repo) | Live Preview |
|---|---------|--------------|----------------|--------------|
| 1 | Camila | Growth & Product Analyst on the WhyNot team. Unlike the app's end users, Camila doesn't shop through WhyNot, she uses its usage data to guide what the team builds next. She needs to know whether price-drop alerts actually lead to purchases, whether wishlist saves translate into real purchase intent, and which product categories drive the most engagement, but that data is currently scattered across logs and dashboards with no clear link between a notification and a resulting sale. Without that visibility, she risks prioritizing features based on guesswork instead of evidence — and she's the one who has to bring leadership a data-backed case for what WhyNot should improve next. | [camila-analytics-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/analytics_persona.html) | [View Live](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS4/analytics_persona.html) |

---

## 3. PAS Hypotheses (Problem–Alternative–Solution)-- Made by Juan Felipe Sáenz

> Submit the identified Problem–Alternative–Solution hypotheses. Teams of 6 submit **at least 12 PAS**. Use the template provided by the course (slides).

| # | Problem | Alternative(s) (current workaround) | Solution (proposed) |
|---|---------|--------------------------------------|----------------------|
| 1 | Users save products they are interested in across different places, making them difficult to find later. | They use screenshots, browser tabs, shopping carts, saved social-media posts, bookmarks, personal notes, or platform-specific wishlists. | WhyNot provides one centralized place where users can save products from different stores and platforms. |
| 2 | Users often save only a product link and later do not remember what the link refers to without opening it. | They paste URLs into personal WhatsApp chats, notes, or bookmarks and manually open them later to identify the product. | WhyNot automatically captures and stores relevant product information such as name, image, price, store, and link. |
| 3 | Users repeatedly check product prices because they do not know when an item becomes cheaper. | They manually revisit product pages, saved links, Google Flights, Steam wishlists, or other store-specific tools to check for price changes. | WhyNot tracks saved-product prices and notifies users when the price drops or reaches a target price. |
| 4 | Users may miss discounts because they do not check product prices frequently enough. | They rely on occasional manual checks, retargeted advertisements, store promotions, or chance encounters with the product again. | WhyNot sends timely price-drop and sale alerts so users can identify purchasing opportunities without constant manual checking. |
| 5 | Users have difficulty organizing products from different categories when everything is stored together. | They keep products mixed across screenshots, tabs, chats, carts, or separate platform-specific lists. | WhyNot allows users to create and manage multiple wishlists or categories such as clothes, technology, gifts, or travel. |
| 6 | Manually organizing every saved product can become tedious and may discourage users from maintaining their lists. | Users either leave items unorganized or manually sort them across folders, chats, screenshots, tabs, or different wishlists. | WhyNot can automatically categorize saved products based on their title, store, or product information. |
| 7 | Users who discover products visually may struggle to recognize or remember them when they are stored only as text or links. | They save screenshots or social-media posts because images help them remember the product. | WhyNot provides an image-first view of saved products and stores each item with its product image. |
| 8 | Users compare similar products manually across multiple stores, which can be time-consuming and overwhelming. | They open several tabs, search different stores, and compare prices, reviews, quality, shipping, warranties, or product details on their own. | WhyNot brings saved alternatives together and supports comparison across stores, including price-based comparison. |
| 9 | Users do not always know whether a current price is actually a good deal. | They rely on memory, repeated manual checks, or external tools available only for certain product categories. | WhyNot stores price history and helps users evaluate whether the current price is low relative to previous prices. |
| 10 | Users may lose interest in products over time but still keep them saved, creating clutter and making lists less useful. | They simply ignore old screenshots, links, tabs, carts, or wishlist entries until they are forgotten. | WhyNot can identify stale items and remind users to review whether they are still interested in them. |
| 11 | Users may save the same or very similar product more than once from different sources, creating duplicated information. | They keep duplicate screenshots, tabs, links, or saved posts and manually recognize duplicates later. | WhyNot can detect duplicate or repeated product entries and help users consolidate them. |
| 12 | Users have different privacy preferences and may not want all saved products or wishlists to be shared. | They keep their shopping information private in personal chats, screenshots, private wishlists, or individual accounts and avoid sharing lists. | WhyNot keeps wishlists private by default and allows users to control whether specific items are shared. |

---


## 4. Context Canvas

> Submit the Context Canvas for the proposed solution. Use the template provided by the course (Chapter 3 of the book).

*(To be completed by the team — insert the filled-in Context Canvas image or embedded diagram here, following the same "source + live preview" pattern as the personas if built as an HTML template.)*

---

## 5. Business Questions
| # | Type | Question | Persona it matters to | Data source needed |
|---|------|----------|------------------------|----------------------|
| 1 | Type 1 | In which cities and geographic zones is app usage concentrated, and how does the amount of saved product vary across them?  | Camila | Approximate user location, city or zone, new app logins, # of active sessions, # of saved products. |
| 2 | Type 2 | At what stage of product-saving process do users most commonly abandon it? | Camila | Timestamps and event logs which gather all the process information. |
| 3 | Type 2 | Which method of saving a product allows users to complete the process in less time and with fewer errors? | Camila | Timestamps and event logs which gather all the process information.|
| 4 | Type 2 | Which search paths allow users to find a product quicker?  | Camila | Events (Screen views, filters applied, search performed), 'not found' searches, Timestamps. |
| 5 | Type 2 | What frequency and type of notification 'The price has changed' notification generate more useful app openings without incrementing notification deactivations?.  | Camila | Notifications sent, frequency, magnitude of the price change, # of app openings, # of notifications discards.  |
| 6 | Type 3 | Which unsupported stores do users try to add most frequently, that should be priorized for next updates? | Camila | Unrecognized domains, failed attempts to save, manually registered stores, # of users per store.    |
| 7 | Type 3 | Which secondary features are used less regularly? and if new, with less user adoption? | Camila | First use register, regular use registers, time since last use.  |
| 8 | Type 3 | Which types of automatically extracted data from the products are corrected more frequently?  | Camila | Original result fromm the extraction, missing fields, manual changes before and after saving, origin store, extraction mistakes |
| 9 | Type 4 | Which combinations of store, category and price range concetrate the most amount of purchases and offer the best sales potential for partnerships? | Camila | Saved products by category, store and price; # of unique interested users; clicks to the store, purchases related with the app  |
| 10 | Type * | Which discount notifications generate more related purchases and a higher user retention in the next 30 days segmented by store, category and % of discount? | Camila | Price history, notiification sent, rate of opened notification, product visit, quit click, confirmed purchase. |


---

## 6. VD Map

> Provide a VD Map that displays all 10 business questions defined above. The data sources used must be obtainable through the designed solution or must be publicly available.
<img width="2825" height="1415" alt="VD-map" src="https://github.com/user-attachments/assets/210bb096-4d23-466d-81ba-19a78d7ccab7" />


---

## References

- Lim, Y. K., Stolterman, E., & Tenenberg, J. (2008). *The Anatomy of Prototypes.* ACM TOCHI, 15(2), 1–27. https://doi.org/10.1145/1375761.1375762
- Qualaroo — [Customer Journey Map guide](https://qualaroo.com/customer-journey-map/)
