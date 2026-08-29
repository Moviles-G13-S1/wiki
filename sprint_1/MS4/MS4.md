# MS4 – Integrating Analytics

Team: #13

Members: Juliana Duran 202220671, Santiago Casasbuenas 202214932, Martin Riveira 202321727, Jeronimo Franco 202222204, Juan Felipe Saenz 202311148, Miguel Angel Velandia 202312487.

---

## 1. Problem & Solution Description

> Write two short descriptions: one for the problem selected and one for the proposed solution.

**Problem:** People frequently find products they are interested in across different online stores and social media platforms but are not ready to buy them immediately. As a result, these products become scattered across screenshots, browser tabs, shopping carts, saved posts, etc. making them difficult to find, organize, compare, and track over time. Users may also miss good purchasing opportunities because they have to manually check whether prices have changed. There is a clear lack of a central platform or system where users can easily manage their shopping prospects, and save as much money as possible. 

**Solution:** WhyNot is a mobile application that provides a centralized place where users can save and organize products from different stores and platforms. Each saved product can include information such as its name, image, price, store, link, and category. The app also tracks product prices and can notify users when an item drops in price, goes on sale, or reaches a target price, helping users compare alternatives and make more informed purchasing decisions without constantly checking multiple websites, saving the user time and frustration.

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
| 12 | Users have different privacy preferences and may not want all saved products or wishlists to be shared. | They keep their shopping information private in personal chats, screensho  ts, private wishlists, or individual accounts and avoid sharing lists. | WhyNot keeps wishlists private by default and allows users to control whether specific items are shared. |

---


## 4. Context Canvas - Made By Miguel Velandia

> Submit the Context Canvas for the proposed solution. Use the template provided by the course (Chapter 3 of the book).

<img width="1920" height="1080" alt="context_canvas pptx (1)" src="https://github.com/user-attachments/assets/639bed2e-9c33-442f-b3da-001e52b83e63" />

---

## 5. Business Questions
| # | Type | Question | Why is it important?| Data source needed |
|---|------|----------|------------------------|----------------------|
| 1 | Type 1 | How many errors does the app produce weekly?  | Measures application stability, reveals trends, and helps prioritize fixes. | Error-monitoring logs grouped by week, error type, app version, device, and environment. |
| 2 | Type 2 | How much money do users have sabed by buying through the app? | Quantifies the app’s financial value to users and supports retention and marketing decisions.  | Purchase price, reference price, discounts, completed purchases, currency, and user ID. |
| 3 | Type 2 | Which type of notification is most clicked? | Identifies the messages that generate the most engagement and informs the notification strategy |Notification type, delivery status, impressions, clicks, user ID, and timestamp. |
| 4 | Type 2 | How many clicks does it take a user to save a product?  | Detects friction in a core user journey and highlights opportunities to simplify it. | Clickstream or funnel events from scan/search to successful save, including abandoned attempts. |
| 5 | Type 2 |How many products does a user has saved? | Measures adoption and engagement with a core feature and supports user segmentation. |  Product-save events, current saved-product records, user ID, product ID, and timestamp. |
| 6 | Type 3 | How often do users manually add a produt? | Reveals gaps in automatic recognition, catalog coverage, and store support. | Unrecognized domains, failed attempts to save, manually registered stores, # of users per store.    |
| 7 | Type 3 | Which features are less used? | Helps identify low-value, hard-to-find, or poorly designed features and guides product investment. | Feature usage events, feature exposure, sessions, unique users, completion rates, and timestamps. |
| 8 | Type 3 | Which types of automatically extracted data from the products are corrected more frequently?  | Identifies unreliable extraction fields and helps prioritize model or rule improvements. | Original result fromm the extraction, missing fields, manual changes before and after saving, origin store, extraction mistakes |
| 9 | Type 4 | Which category has the most amount of purchases per month? | Shows demand by category and informs partnerships, promotions, and catalog priorities. |  Completed purchases with category, product, user, price, store, and purchase date. |
| 10 | Type * |What are the users buying patterns? | Supports personalization, recommendations, forecasting, and retention initiatives. |  Purchase history by user, product, category, store, price, quantity, timestamp, and repeat-purchase interval  |
  

---

## 6. VD Map

> Provide a VD Map that displays all 10 business questions defined above. The data sources used must be obtainable through the designed solution or must be publicly available.
<img width="2785" height="1436" alt="foto" src="https://github.com/user-attachments/assets/049a0591-754d-4365-990e-ea989cd315ed" />



---

## References

- Lim, Y. K., Stolterman, E., & Tenenberg, J. (2008). *The Anatomy of Prototypes.* ACM TOCHI, 15(2), 1–27. https://doi.org/10.1145/1375761.1375762
- Qualaroo — [Customer Journey Map guide](https://qualaroo.com/customer-journey-map/)
