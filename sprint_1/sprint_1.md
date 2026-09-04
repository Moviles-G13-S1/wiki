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

## 2. Sprint 1 Pending Tasks

The rest of this document works through the [Sprint 1 Pending Tasks](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/Sprint%201%20Pending%20Tasks.md) checklist, **in the order listed there**.

### 1. Revenue Model & Value Proposition — `[Wiki Content]`

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

## 5. Business Questions
| # | Type | Question | Why is it important?| Data source needed |
|---|------|----------|------------------------|----------------------|
| 1 | Type 1 | How many errors does the app produce weekly?  | Measures application stability, reveals trends, and helps prioritize fixes. | Error-monitoring logs grouped by week, error type, app version, device, and environment. |
| 2 | Type 1 | What is the average loading time of the home screen? | Measures how optimized is the app | Timestamps and time record logs from the apps homescreen |
| 3 | Type 2 | How much money have users saved on the products they marked as purchased in the app? | Quantifies the app’s financial value to users and supports retention and marketing decisions.  | Purchase price, reference price, discounts, completed purchases, currency, and user ID. |
| 4 | Type 2 | Which type of notification is most clicked? | Identifies the messages that generate the most engagement and informs the notification strategy |Notification type, delivery status, impressions, clicks, user ID, and timestamp. |
| 5 | Type 2 | How many clicks does it take a user to save a product?  | Detects friction in a core user journey and highlights opportunities to simplify it. | Clickstream or funnel events from scan/search to successful save, including abandoned attempts. |
| 6 | Type 2 |How many products does a user has saved? | Measures adoption and engagement with a core feature and supports user segmentation. |  Product-save events, current saved-product records, user ID, product ID, and timestamp. |
| 7 | Type 3 | How often do users manually add a produt? | Reveals gaps in automatic recognition, catalog coverage, and store support. | Unrecognized domains, failed attempts to save, manually registered stores, # of users per store.    |
| 8 | Type 3 | Which features are less used? | Helps identify low-value, hard-to-find, or poorly designed features and guides product investment. | Feature usage events, feature exposure, sessions, unique users, completion rates, and timestamps. |
| 9 | Type 3 | Which types of automatically extracted data from the products are corrected more frequently?  | Identifies unreliable extraction fields and helps prioritize model or rule improvements. | Original result fromm the extraction, missing fields, manual changes before and after saving, origin store, extraction mistakes |
| 10 | Type 3 | Which method do users prefer for saving a product? (Automatically or manually)  | This allows us to realize if it is worth maintaining both features or if its unnecessary  | User logs for each time the a product is saved manually vs automatically |
| 11 | Type 4 | Which category has the highest number of products marked as purchased per month? | Shows demand by category and informs partnerships, promotions, and catalog priorities. |  Marked purchases with category, product, user, price, store, and purchase date. |
| 12 | Type 4 | What is the demographic profile of the average buyer per category? | This allows us to realize which type of users buy a specific type of product | Marked purchases with category, product, user, price, store, and purchase date. |
| 13 | Type * |What are the buying patterns of users based on products they have marked as purchased? | Supports personalization, recommendations, forecasting, and retention initiatives. |  Purchase history by user, product, category, store, price, quantity, timestamp, and repeat-purchase interval  |
| 14 | Type * | Is there a relationship between the number of errors a user experiences and the number of products they save?  | Allows us to recognize the impact of the errors the app is having  | Error logs and Saved products per user |
  
  

---

## 6. VD Map

> Provide a VD Map that displays all 10 business questions defined above. The data sources used must be obtainable through the designed solution or must be publicly available.
<img width="3152" height="1268" alt="upadartedvdmap jpg" src="https://github.com/user-attachments/assets/59925d69-898e-4352-a4e5-93a63c647212" />

**Notes on relationships / data sources**

*(Optional — use this space to note anything about how questions relate to each other or share a data source, useful context for whoever reviews the map.)*

---

### 4. Functional Scenarios — `[5 individual points]` 

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

### 5. Quality Scenarios — `[5 individual points]` 

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

### 6. Ethics Video — `[46 team points]`

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

### 7. Repository Tools & Collaboration — `[Process + Team Evaluation]`

Current snapshot of the repo (`Moviles-G13-S1/wiki`) as of this check: **0 open issues**, **2 pull requests**, **0 milestones**. This section needs real process evidence — a Kanban board tracking the remaining tasks, Issues assigned per person, a Sprint 1 Milestone, and Pull Requests (reviewed by a teammate) for any further changes — so that all 6 members show visible contribution before the deadline.

**Kanban / Project board link**

Sprint 1 project board: https://github.com/orgs/Moviles-G13-S1/projects/7

MicroSprints project boards:

- MS2: https://github.com/orgs/Moviles-G13-S1/projects/4
- MS3: https://github.com/orgs/Moviles-G13-S1/projects/5
- MS4: https://github.com/orgs/Moviles-G13-S1/projects/6

**Milestone link**

https://github.com/Moviles-G13-S1/wiki/milestone/1


**Notes on task assignment / ownership**

*(Optional — useful if it's not already obvious from the Issues themselves.)*

---

### 8. Final Sprint 1 Report

This section (and this whole file) is the working source for the final report. Once revenue model, value proposition, the 14 business questions, and the updated VD map above are filled in, consolidate everything — together with what's already finished (functional & quality scenarios) — into a single Markdown page and publish it on the **GitHub Wiki** (`/wiki` tab), since that's what actually gets submitted via Bloque Neón, not this repo's main branch.

**Status notes**

*(Paste anything relevant here — e.g. "consolidated on [date], published to wiki at [link]".)*

---

### 9. Artifact Quality — `[20 individual points]`

A final pass over everything above before submission: proofreading, consistent terminology/headings/tables/image sizing, high-resolution images, and no placeholder text left behind. Also worth testing every link in this document and the linked pages — the persona table currently links via `htmlpreview.github.io`, which has been unreliable; consider switching to `raw.githack.com` (used throughout this document) instead.

**Review notes**

*(Paste anything found during the final proofreading pass here — broken links, inconsistent formatting, leftover placeholder text, etc.)*

---

## Final Submission Check
- [ ] Confirm that every pending artifact is complete.
- [ ] Confirm that all 6 team members reviewed the final report.
- [ ] Confirm that repository collaboration evidence is visible.
- [ ] Update the GitHub Project/Kanban.
- [ ] Close completed Issues.
- [ ] Merge the final Pull Requests.
- [ ] Verify the final Wiki/repository link.
- [ ] Submit the required link through Bloque Neón **before September 5th, 2026 at 5:00 am**.
- [ ] Do not edit the graded report after the deadline.
