# Sprint 1 — WhyNot

**Team:** #13
**Members:** Juliana Duran 202220671, Santiago Casasbuenas 202214932, Martin Riveira 202321727, Jeronimo Franco 202222204, Juan Felipe Saenz 202311148, Miguel Angel Velandia 202312487.

**Project:** WhyNot — a wishlist and smart shopping app that helps users save, organize, and track products they want to buy in one place.
**Interactive prototype:** https://why-not-wish-shop.lovable.app

> **Note:** this file consolidates and links to Sprint 1's working documents in the repo (the drafting/evidence archive). Per the course's submission rules, the actual graded deliverable must be published as Markdown on the **GitHub Wiki** (`/wiki` tab) and submitted via Bloque Neón — this file is the source used to assemble that final page.

---

## 1. Microsprints

### [MS2 — Design Thinking Process Practice](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS2/MS2.md)
The starting point of the sprint: the team selected 4 candidate problems, conducted 7 user interviews (recordings + transcripts in `MS2/evidence/`), extracted What–How–Why situations from each, built journey maps, and ran an initial brainstorming pass that led toward the WhyNot concept.
[Deliverable checklist](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS2/MS2_Deliverable_Checklist.md)

### [MS3 — Defining a Solution](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/MS3.md)
Converged on WhyNot as the selected solution. Includes the brainstorming/decision process used to pick the idea, 5 empathy maps (one per prospective user), and 3 personas — Emilio, Carlos, and Andrea — each covering a different core use case (universal wishlist, careful comparison shopping, and deal discovery).
[Emilio](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS3/personas/emilio-persona.html) · [Carlos](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS3/personas/carlos-persona.html) · [Andrea](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS3/personas/persona-andrea.html) · [Persona link table](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/persona_table.md)
[Deliverable checklist](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/MS3_Deliverable_Checklist.md)

### [MS4 — Integrating Analytics](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/MS4.md)
Added the analytics layer to the design: the problem/solution statement, an analytics persona (Camila, Growth & Product Analyst), 12+ PAS hypotheses, a Context Canvas, an initial set of 10 business questions, and a first VD Map.
[Camila — analytics persona](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS4/analytics_persona.html)
[Deliverable checklist](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/MS4_Deliverable_Checklist.md)

### App Reports
Two subteam app-analysis reports are tracked under [`app_reports/`](https://github.com/Moviles-G13-S1/wiki/tree/main/sprint_1/app_reports) ([subteam 1](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/app_reports/subteam_1_app_report.md), [subteam 2](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/app_reports/subteam_2_app_report.md)) — both files currently exist but are still empty and need to be filled in.

---

## 2. Problem, Solution, Value Proposition and Revenue Model

Describe how WhyNot makes money, and the core value it delivers to users. Both should stay consistent with the problem/solution statement already written in [MS4.md](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/MS4.md#1-problem--solution-description).

**Revenue Model**

Saving products and tracking prices stays free — that's the whole point of WhyNot, and charging for it would kill adoption. Instead, money comes in around the moment a saved item actually becomes worth buying:
- **Affiliate commissions.** When a price alert leads a user to tap through and buy, WhyNot earns a small cut from the store's affiliate program (the same deep-link back to the store that FS2 already uses). No purchase, no revenue.
- **WhyNot Plus.** A paid tier for people who want more: unlimited active price alerts, faster price checks, full price-history charts, and comparison across saved alternatives — mostly what Carlos and Andrea would pay for.
- **Sponsored deals.** Stores can pay to surface a relevant sale to users tracking that category, clearly labeled and shown inside the normal deals feed instead of as separate ads.

**Value Proposition**

WhyNot is the one place to save anything you're interested in buying — from any store — and get told the moment it's actually worth pulling the trigger. It replaces screenshots, open tabs, and forgotten carts with a list that watches prices for you, something a bookmark or a single store's wishlist can't do. It's why Emilio can keep everything in one place regardless of store or category, why Andrea gets pinged the second her target price hits, and why Carlos gets the price history he needs to know a deal is real.

**Consistency check**

Both tie back to the MS4 problem/solution: products get scattered with no way to track their prices, and WhyNot's answer is a centralized wishlist that does the tracking. The revenue model just monetizes the purchase that solution already leads to, so users never pay for the core saving/tracking WhyNot promises them.

---

## 3. PAS – Problem–Alternative–Solution Structure
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

## 4. Context Canvas

<img width="1920" height="1080" alt="context_canvas pptx (1)" src="https://github.com/user-attachments/assets/639bed2e-9c33-442f-b3da-001e52b83e63" />

---

## 5. Personas

| # | Persona | Image | Description | Source (repo) | Live Preview | Done By |
|---|---------|-------|-------------|---------------|--------------|---------|
| 1 | Emilio | <img src="personas/Emilio.jpeg" width="160"> | 23-year-old student at Universidad de los Andes; shops mainly for books and clothes, tracks items only via an Amazon wishlist | [emilio-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/emilio-persona.html) | [View live](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS3/personas/emilio-persona.html) | Santiago Casasbuenas |
| 2 | Carlos | <img src="personas/Carlos.jpeg" width="160"> | Carlos is a practical, budget-conscious online shopper who carefully compares prices, reviews, and product quality before making confident purchasing decisions. | [carlos-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/carlos-persona.html) | [View live](https://htmlpreview.github.io/?https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/carlos-persona.html) | Jeronimo Franco |
| 3 | Andrea | <img src="personas/Andrea.jpeg" width="160"> | Andrea is an independent young woman who already works and lives alone. She enjoys shopping online more than in person, and she enjoys saving money on new items she hadn't noticed before. | [andrea-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/persona-andrea.html) | [View live](https://htmlpreview.github.io/?https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/persona-andrea.html) | Martin Riveira |

---

## 6. Empathy Maps

| # | Persona | Link to Map | Done By |
|---|---------|--------------|--------|
| 1 | Emilio | [Emilio's Map](https://app.mural.co/t/moviles6182/m/moviles6182/1787240133659/a180902d884db9882945da525c3f2607154be4f5) | Santiago Casasbuenas |
| 2 | Cristian | [Cristian´s Map](https://app.mural.co/t/empathy8461/m/empathy8461/1787101645013/fe0c5b0c2bf319c69dc822522b384f8d3086f41f?sender=ud3159237ac70835f8a485549) | Juan Felipe Sáenz |
| 3 | Violeta | [Violetas's Map](https://app.mural.co/t/moviles6182/m/moviles6182/1787108433558/85f2e7cb0722de4687f1705bd265d63e663ca08a?sender=ua1041bd0f93ddc7c5a9d7309) | Juliana Durán |
| 4 | Carlos | [Carlos's Map](https://app.mural.co/t/moviles6182/m/moviles6182/1787316143105/f09ac0679078f12322e66ae8967fd6cb4f49960c?sender=udb71de2dc78dff2ddb853584) | Jeronimo Franco |
| 5 | Andrea | [Andrea's Map](https://app.mural.co/t/work48123/m/work48123/1787329701926/5a1e2da2761fbd10e5a2b9564538a675aedc4d20) | Martin Riveira |

### Empathy Map 1 - Emilio

**Persona description:** Emilio, 23 years old. Student at Universidad de los Andes. Mainly shops online for books and clothes. Browses online stores/social media about once a week. Uses an Amazon wishlist only for books, nothing for clothes. Compares products mainly by price. Prefers to keep his wants and lists private. Gets easily overwhelmed by too much information.

<img width="662" height="707" alt="image" src="https://github.com/user-attachments/assets/10590a76-7e8d-4bdd-a364-982e3681c074" />

**Evidence:** [Full interview transcript](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS2/evidence/interview-1/transcript.md)

### Empathy Map 2 — *Cristian*
**Persona Description:** Cristian, 19 years old. Mainly shops online for video games and technology products. Browses online stores occasionally, around once or twice a month. Uses Steam wishlists for games and saves other product links in his personal WhatsApp chat. Compares products mainly by price and quality. Often waits for discounts before buying and prefers to keep his wishlists private. Values price alerts because he dislikes having to repeatedly check whether prices have changed.

<img width="470" height="504" alt="image" src="https://github.com/user-attachments/assets/8d082ef7-0da2-4563-8892-20d284e276ec" />


### Empathy Map 3 — *Violeta*
**Persona Description:** Violeta, 25 years old. Has a full-time job and enjoys fashion and shopping. Frequently browses online stores and social media to discover new products. Often finds things she likes but does not buy them immediately. Saves products across screenshots, shopping carts, open tabs, and social media. Likes comparing different options and prices before making a purchase. Wants to find good deals and make smarter purchasing decisions.

<img width="588" height="715" alt="image" src="https://github.com/user-attachments/assets/7866cf7b-40c0-4271-a5b6-bc9b312666b5" />


### Empathy Map 4 — *Carlos* 
**Persona Description:**
Carlos is a 29-year-old practical online shopper who carefully researches electronics, household products, and gifts before buying. He compares prices, reviews, quality, shipping, and warranties across multiple stores, often saving products in tabs, bookmarks, or screenshots while waiting for a better deal. Although too many options can overwhelm him, he feels confident when he finds a durable, reliable product at a fair price.
<img width="6347" height="4766" alt="Carlos - Empathy map_2026-08-21_12-57-53" src="https://github.com/user-attachments/assets/33cb65b6-b9a0-42f2-996c-ead8d37ee174" />


### Empathy Map 5 — *_Andrea_*
Andrea is a 29-year-old administrator and frequent online shopper who enjoys finding good deals and discovering new products that match her interests. She mainly shops online, often compares prices across different stores, and likes being notified about discounts before they disappear. Because she travels frequently and does not want to constantly check multiple websites or apps, she values simple, personalized alerts that bring relevant offers and new products directly to her. She enjoys the feeling of saving money, but feels frustrated when she misses a deal or finds out about it too late.
<img width="929" height="1128" alt="image" src="https://github.com/user-attachments/assets/4242fab2-4cb4-47df-a563-bea7ecff07ee" />

---

## 7. Business Questions

| # | Type | Question | Why is it important?| Data source needed |
|---|------|----------|------------------------|----------------------|
| 1 | Type 1 | How many errors does the app produce weekly?  | Measures application stability, reveals trends, and helps prioritize fixes. | Error-monitoring logs grouped by week, error type, app version, device, and environment. |
| 2 | Type 2 | How much money have users saved on the products they marked as purchased in the app? | Quantifies the app’s financial value to users and supports retention and marketing decisions.  | Purchase price, reference price, discounts, completed purchases, currency, and user ID. |
| 3 | Type 2 | Which type of notification is most clicked? | Identifies the messages that generate the most engagement and informs the notification strategy |Notification type, delivery status, impressions, clicks, user ID, and timestamp. |
| 4 | Type 2 | How many clicks does it take a user to save a product?  | Detects friction in a core user journey and highlights opportunities to simplify it. | Clickstream or funnel events from scan/search to successful save, including abandoned attempts. |
| 5 | Type 2 |How many products does a user has saved? | Measures adoption and engagement with a core feature and supports user segmentation. |  Product-save events, current saved-product records, user ID, product ID, and timestamp. |
| 6 | Type 3 | How often do users manually add a produt? | Reveals gaps in automatic recognition, catalog coverage, and store support. | Unrecognized domains, failed attempts to save, manually registered stores, # of users per store.    |
| 7 | Type 3 | Which features are less used? | Helps identify low-value, hard-to-find, or poorly designed features and guides product investment. | Feature usage events, feature exposure, sessions, unique users, completion rates, and timestamps. |
| 8 | Type 3 | Which types of automatically extracted data from the products are corrected more frequently?  | Identifies unreliable extraction fields and helps prioritize model or rule improvements. | Original result fromm the extraction, missing fields, manual changes before and after saving, origin store, extraction mistakes |
| 9 | Type 4 | Which category has the highest number of products marked as purchased per month? | Shows demand by category and informs partnerships, promotions, and catalog priorities. |  Marked purchases with category, product, user, price, store, and purchase date. |
| 10 | Type * |What are the buying patterns of users based on products they have marked as purchased? | Supports personalization, recommendations, forecasting, and retention initiatives. |  Purchase history by user, product, category, store, price, quantity, timestamp, and repeat-purchase interval  |

---

## 8. VD Map

<img width="3152" height="1268" alt="upadartedvdmap jpg" src="https://github.com/user-attachments/assets/59925d69-898e-4352-a4e5-93a63c647212" />

---

## 9. Functional Scenarios (FS)

Covers the main WhyNot functionalities (universal wishlist, price tracking & alerts, product comparison, personalized discovery) and stays consistent with the proposed solution — no further action needed here unless the solution description changes.

#### **FS1 — Saving an item from any category**
- **Persona:** Emilio
- **User action:** While browsing a clothing site on his phone, Emilio taps "Save to WhyNot" on a pair of sneakers he's considering.
- **System response:** WhyNot adds the item to his unified wishlist regardless of category, stores its current price and image, and confirms with a brief toast.
- **Execution context:** Emilio is on mobile data, logged in, and this is the first time he's saved a clothing item — previously he only tracked books through Amazon's separate list.

#### **FS2 — Returning directly to the product page**
- **Persona:** Emilio
- **User action:** A week later, Emilio opens WhyNot and taps the saved sneakers in his wishlist.
- **System response:** WhyNot deep-links straight to the original store's product page, with no need to search again.
- **Execution context:** Emilio is on home Wi-Fi; the item is still in stock and the price is unchanged.

#### **FS3 — Checking regional availability before saving**
- **Persona:** Emilio
- **User action:** Emilio finds a product on a US-based retailer's site he hasn't used before and wants to know if it ships to Colombia before saving it.
- **System response:** WhyNot flags shipping availability to Colombia directly on the save-confirmation screen, based on store metadata.
- **Execution context:** Emilio is browsing an unfamiliar international store for the first time.

#### **FS4 — Setting a target price**
- **Persona:** Andrea
- **User action:** Andrea saves a dress to her wishlist and sets a target price 20% below the current one.
- **System response:** WhyNot stores the target and begins monitoring the item, ready to notify her once the price reaches or drops below it.
- **Execution context:** Andrea sets this up on mobile data during a lunch break, ahead of a weekend trip.

#### **FS5 — Receiving a price-drop notification**
- **Persona:** Andrea
- **User action:** Andrea receives a push notification: "Your saved dress just dropped to $85,000 (target reached)."
- **System response:** WhyNot triggers the push and updates the item's status to "Deal available" in her wishlist.
- **Execution context:** Andrea is traveling abroad, connected to hotel Wi-Fi, outside normal business hours.
  
#### **FS6 — Customizing notification preferences**
- **Persona:** Andrea
- **User action:** In Settings, Andrea disables "general promotions" but keeps "price-drop alerts for saved items" on.
- **System response:** WhyNot updates her preferences immediately, stopping generic promo pushes while continuing price-drop alerts.
- **Execution context:** Andrea does this after her first week using the app, having felt overwhelmed by irrelevant notifications.
  
#### **FS7 — Passive price recheck without opening the app daily**
- **Persona:** Emilio
- **User action:** Emilio opens the app once during the week; he never manually rechecks prices.
- **System response:** WhyNot has already run a background price check that morning and shows a "price changed" badge on two saved items.
- **Execution context:** Background app refresh is enabled; the check ran automatically before Emilio opened the app.

#### **FS8 — Comparing two saved products side-by-side**
- **Persona:** Carlos
- **User action:** Carlos selects two saved blenders from his wishlist and taps "Compare."
- **System response:** WhyNot displays a side-by-side view of price, rating, and key specs for both.
- **Execution context:** Carlos is deciding between the two at night, using WhyNot's web/laptop view.

#### **FS9 — Viewing warranty and return info on a saved product**
- **Persona:** Carlos
- **User action:** Carlos taps the "Details" tab on a saved laptop.
- **System response:** WhyNot shows a consolidated summary of warranty length, shipping time, and return policy pulled from the retailer's page.
- **Execution context:** Carlos is close to purchasing and wants to confirm the return policy before committing, on mobile.

#### **FS10 — Reading an aggregated review summary while saving**
- **Persona:** Carlos
- **User action:** Carlos saves a new espresso machine and taps "Reviews."
- **System response:** WhyNot pulls and displays review scores/summaries from the linked store, instead of requiring separate tabs.
- **Execution context:** Carlos is in the early research phase with several browser tabs already open, looking for a faster way to gauge reliability.

#### **FS11 — Discovering a relevant deal via the home feed**
- **Persona:** Andrea
- **User action:** Andrea opens the WhyNot home feed with no specific search intent.
- **System response:** WhyNot surfaces a discount on a brand she follows, based on her stated interests and past saves.
- **Execution context:** Andrea has already completed her interest profile; she's browsing casually.

#### **FS12 — Following a brand for future alerts**
- **Persona:** Andrea
- **User action:** After saving an item, Andrea taps "Follow" on that brand's page inside WhyNot.
- **System response:** WhyNot adds the brand to her followed list and includes its future promotions in her personalized feed and notifications.
- **Execution context:** Andrea just discovered the brand through a saved item and wants ongoing updates without repeat manual searching.



---

## 10. Quality Scenarios (QS)

12 quality scenarios were written, each covering a distinct quality attribute (eventual connectivity, performance, resilience, notification load, internationalization, energy efficiency, security/privacy, accessibility, data consistency, GUI responsiveness, usability, scalability), in the same document as the functional scenarios above.

Each scenario follows: **Scenario name → Quality attribute(s) → App status and context → Change in the context → System reaction.**
 
#### **QS1 — Price sync interrupted mid-check**
- **Quality attribute:** Eventual connectivity
- **App status and context:** WhyNot is running a scheduled background price check across Emilio's 15 saved items.
- **Change in context:** Emilio's phone loses connectivity mid-sync (e.g., entering the subway).
- **System reaction:** WhyNot pauses the sync, queues the remaining checks, and resumes automatically once connectivity returns — without showing stale prices as if they were current.
  
#### **QS2 — Large wishlist load time**
- **Quality attribute:** Performance
- **App status and context:** Carlos has 150+ saved products across multiple categories.
- **Change in context:** Carlos opens the wishlist screen and scrolls quickly through all items.
- **System reaction:** WhyNot loads the list within 2 seconds using pagination/lazy-loading, without freezing the UI or dropping frames.

#### **QS3 — Comparison with missing product data**
- **Quality attribute:** Resilience
- **App status and context:** Carlos compares two products, one of which has incomplete specification data from the retailer's API.
- **Change in context:** A spec field returns an error/null from the source.
- **System reaction:** WhyNot displays "Information not available" for that field instead of crashing or showing a broken comparison view.

#### **QS4 — Flash-sale notification spike**
- **Quality attribute:** Usability / notification load management
- **App status and context:** Andrea follows 20 brands and has price alerts on 30 items.
- **Change in context:** A flash-sale event triggers 40 price-drop conditions within the same hour.
- **System reaction:** WhyNot batches the alerts into a single grouped notification ("12 of your saved items just dropped in price") instead of sending 40 separate pushes.

#### **QS5 — Notifications across time zones while traveling**
- **Quality attribute:** Internationalization / context-awareness
- **App status and context:** Andrea is traveling internationally; her phone's timezone has auto-updated.
- **Change in context:** A price-drop alert triggers for a saved item.
- **System reaction:** WhyNot delivers time-sensitive price-drop alerts immediately, but holds non-urgent grouped promos until outside her local 10pm–7am quiet hours.

#### **QS6 — Background checks under low battery**
- **Quality attribute:** Energy efficiency
- **App status and context:** WhyNot runs periodic background price checks for all users.
- **Change in context:** Emilio's battery drops below 20%.
- **System reaction:** WhyNot reduces background price-check frequency (e.g., hourly → every 6 hours) to conserve battery, resuming normal frequency once charging or above threshold.

#### **QS7 — Private wishlist protection**
- **Quality attribute:** Security / privacy
- **App status and context:** Emilio has marked his wishlist as private and disabled sharing.
- **Change in context:** Another WhyNot user tries to view Emilio's profile/wishlist.
- **System reaction:** WhyNot blocks visibility and returns "This wishlist is private," without exposing any item data.

#### **QS8 — Accessible product comparison**
- **Quality attribute:** Accessibility
- **App status and context:** Carlos uses a screen reader due to low vision.
- **Change in context:** Carlos navigates to the side-by-side comparison screen with VoiceOver/TalkBack active.
- **System reaction:** WhyNot announces each product's key attributes in a logical reading order and labels all interactive elements, so Carlos can complete the comparison without visual cues.

#### **QS9 — Cross-device data consistency**
- **Quality attribute:** Data consistency
- **App status and context:** Carlos has WhyNot open on both his laptop and phone at the same time.
- **Change in context:** He updates a target price on his phone.
- **System reaction:** WhyNot syncs the change to his laptop session within a few seconds, keeping both devices consistent.

#### **QS10 — Readability in bright outdoor light**
- **Quality attribute:** GUI responsiveness / usability
- **App status and context:** Andrea opens WhyNot outdoors in bright sunlight to check a deal.
- **Change in context:** The ambient light sensor detects high brightness.
- **System reaction:** WhyNot increases contrast and suggests a high-contrast display mode so text and price info stay legible.

#### **QS11 — Simplifying an overloaded spec view**
- **Quality attribute:** Usability
- **App status and context:** Emilio views a product's full spec sheet, which shows a large number of fields by default.
- **Change in context:** Emilio taps to collapse it into an "essentials only" view.
- **System reaction:** WhyNot immediately re-renders the screen showing only price, availability, and one key differentiator — no reload required.
  
#### **QS12 — Peak traffic during a sale event**
- **Quality attribute:** Scalability
- **App status and context:** A major regional sale event causes a spike in concurrent users checking prices.
- **Change in context:** Concurrent price-check requests increase roughly 10x above normal load.
- **System reaction:** WhyNot's backend auto-scales to handle the load, keeping price-check response times under an acceptable threshold (e.g., 3 seconds) without dropping requests.

---

### 11. Ethics Video

A 5–10 minute video covering the ethical considerations relevant to WhyNot and this sprint.

**Ethical considerations identified**

*(Paste here — e.g. price-tracking data privacy, how affiliate revenue might bias recommendations, targeting/notification fatigue, etc.)*

**Script / structure outline**

*(Paste here.)*

**Team participation**

*(Note here who does what — on-camera, editing, script, etc.)*

**Final video link**

*(Paste the published link here once recorded and edited. Confirm duration is between 5–10 minutes before pasting.)*

---


# Revisar. Artifact Quality — `[20 individual points]`

A final pass over everything above before submission: proofreading, consistent terminology/headings/tables/image sizing, high-resolution images, and no placeholder text left behind. Also worth testing every link in this document and the linked pages — the persona table currently links via `htmlpreview.github.io`, which has been unreliable; consider switching to `raw.githack.com` (used throughout this document) instead.

**Review notes**

*(Paste anything found during the final proofreading pass here — broken links, inconsistent formatting, leftover placeholder text, etc.)*

---
