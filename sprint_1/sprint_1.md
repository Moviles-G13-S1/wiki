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

*(Paste here — e.g. affiliate commissions on tracked purchases, premium subscription tier, sponsored placements, etc. Explain how the mechanism actually works for WhyNot specifically.)*

**Value Proposition**

*(Paste here — what unique value does WhyNot give users that alternatives don't, and to whom specifically.)*

**Consistency check**

*(Note here how the above ties back to the selected problem and proposed solution — one or two sentences is enough.)*

---

### 2. Business Questions — `[10 individual points]`

The final report needs **14 business questions** (Type 1 ≥2, Type 2 ≥4, Type 3 ≥4, Type 4 ≥2, Type 5 ≥2). The current [MS4.md](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/MS4.md#5-business-questions) version has 10, so the table below carries those 10 over and adds open rows for what's missing. Whoever writes a new question, paste it directly into its row — include the question, why it matters, and the data source it needs, same as the existing rows.

| # | Type | Question | Why is it important? | Data source needed |
|---|------|----------|------------------------|----------------------|
| 1 | Type 1 | How many errors does the app produce weekly? | Measures application stability, reveals trends, and helps prioritize fixes. | Error-monitoring logs grouped by week, error type, app version, device, and environment. |
| 2 | Type 2 | How much money do users save by buying through the app? | Quantifies the app's financial value to users and supports retention and marketing decisions. | Purchase price, reference price, discounts, completed purchases, currency, and user ID. |
| 3 | Type 2 | Which type of notification is most clicked? | Identifies the messages that generate the most engagement and informs the notification strategy. | Notification type, delivery status, impressions, clicks, user ID, and timestamp. |
| 4 | Type 2 | How many clicks does it take a user to save a product? | Detects friction in a core user journey and highlights opportunities to simplify it. | Clickstream or funnel events from scan/search to successful save, including abandoned attempts. |
| 5 | Type 2 | How many products has a user saved? | Measures adoption and engagement with a core feature and supports user segmentation. | Product-save events, current saved-product records, user ID, product ID, and timestamp. |
| 6 | Type 3 | How often do users manually add a product? | Reveals gaps in automatic recognition, catalog coverage, and store support. | Unrecognized domains, failed attempts to save, manually registered stores, # of users per store. |
| 7 | Type 3 | Which features are less used? | Helps identify low-value, hard-to-find, or poorly designed features and guides product investment. | Feature usage events, feature exposure, sessions, unique users, completion rates, and timestamps. |
| 8 | Type 3 | Which types of automatically extracted product data are corrected more frequently? | Identifies unreliable extraction fields and helps prioritize model or rule improvements. | Original extraction result, missing fields, manual changes before/after saving, origin store, extraction mistakes. |
| 9 | Type 4 | Which category has the most purchases per month? | Shows demand by category and informs partnerships, promotions, and catalog priorities. | Completed purchases with category, product, user, price, store, and purchase date. |
| 10 | Type * | What are the users' buying patterns? | Supports personalization, recommendations, forecasting, and retention initiatives. | Purchase history by user, product, category, store, price, quantity, timestamp, and repeat-purchase interval. *(Review: reclassify into Type 1–5, or keep as-is?)* |
| 11 | Type 1 | *(Paste the missing Type 1 question here)* | | |
| 12 | Type 3 | *(Paste the missing Type 3 question here)* | | |
| 13 | Type 4 | *(Paste the missing Type 4 question here)* | | |
| 14 | Type 5 | *(Paste a Type 5 question here)* | | |
| 15 | Type 5 | *(Paste a second Type 5 question here)* | | |

*(Once rows 11–15 are filled and row 10 is resolved, confirm the final total is 14 questions and check that every data source is realistically obtainable through WhyNot or is publicly available.)*

---

### 3. VD Map — `[10 individual points]`

The current VD Map (embedded in [MS4.md](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS4/MS4.md#6-vd-map)) covers the 10 questions above. Once the table in section 2 is finalized at 14 questions, rebuild the map to include all of them and export it at a resolution where every node and label stays legible.

**Updated VD Map**

*(Paste the new VD Map image/embed here once ready, replacing the one in MS4.md.)*

**Notes on relationships / data sources**

*(Optional — use this space to note anything about how questions relate to each other or share a data source, useful context for whoever reviews the map.)*

---

### 4. Functional Scenarios — `[5 individual points]` 

**Completed.** 12 functional scenarios were written, grounded in Emilio, Carlos, and Andrea, each following the User Action / System Response / Execution Context framework.

📄 [Functional & Quality Scenarios — WhyNot](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/Functional-Quality-Scenarios.md)

Covers the main WhyNot functionalities (universal wishlist, price tracking & alerts, product comparison, personalized discovery) and stays consistent with the proposed solution — no further action needed here unless the solution description changes.

---

### 5. Quality Scenarios — `[5 individual points]` 

**Completed.** 12 quality scenarios were written, each covering a distinct quality attribute (eventual connectivity, performance, resilience, notification load, internationalization, energy efficiency, security/privacy, accessibility, data consistency, GUI responsiveness, usability, scalability), in the same document as the functional scenarios above.

📄 [Functional & Quality Scenarios — WhyNot](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/Functional-Quality-Scenarios.md)

Clearly differentiated from the functional scenarios above — no further action needed here.

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

*(Paste here once created.)*

**Milestone link**

*(Paste here once created.)*

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
