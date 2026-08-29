# MS3 – Defining a Solution: Problem, Solution, Empathy Maps, and Personas

**Team:** #13

**Members:** Juliana Duran 202220671, Santiago Casasbuenas 202214932, Martin Riveira 202321727, Jeronimo Franco 202222204, Juan Felipe Saenz 202311148, Miguel Angel Velandia 202312487.

---
## 1. Brainstorming Process & New Solutions

> Describe the newly performed brainstorming process, and all the solutions that came from it, including how smart features can be included. Detail the procedure followed to derive the mentioned solutions. The solutions should come from the situations, journey maps, and interviews detailed in the MS2 report. Include evidence (e.g., screenshots) of this task.

### 1.1 Methodology
 
The ideation followed the Brainstorming rules discussed in class — no idea is rejected during generation, no criticism until the divergence phase is closed, quantity over quality in the first pass.
 
**Generation — collaborative board.** The team worked on a shared Miro board where each of the six members contributed one candidate application, written as a sticky note under their own name. Assigning one idea per member was a deliberate choice: it guarantees that every member's perspective is represented in the final set, and it prevents the outcome from being dominated by whoever is most vocal or most invested in a particular domain. The result is a set of six ideas from six people, each traceable to the member who proposed it.
 
Each idea came from the member's own experience or from something they had observed in people around them. The user research came afterwards, not before: the vote narrowed the six ideas down, the course brief allowed only four problem statements to be carried into MS2-O1, and the seven interviews were then conducted to test whether the pain each of those four assumed was real. More interviews were deliberately assigned to the leading idea than to the others, so that the option the team was most likely to build would be the best understood. Section 1.3 records, for every idea, what that research ended up showing.
 
**Selection — asynchronous vote.** Once every idea was on the board, the team deliberately postponed the decision instead of choosing in the heat of the session. The list was taken to the team's group chat the following day, where each member approved every idea they considered viable. Voting a day later, in writing, gave everyone time to weigh the ideas on their own rather than against whoever argued loudest in the session. The vote is documented in Section 2.
 
Separating generation from selection is the core of the divergence–convergence discipline: mixing them causes ideas to be judged before they are fully formulated.

### 1.2 Session description

| Item | Detail |
|------|--------|
| Format | Collaborative brainstorming on a shared Miro board |
| Date | 10-08-2026 |
| Duration | 20 minutes |
| Participants | All six team members, one idea each |
| Facilitator | Juliana Duran |
| Board | [Miro Link](https://miro.com/app/board/uXjVHv5hGls=/?share_link_id=243210882480) |
| Selection | Asynchronous vote in the team's WhatsApp group chat |
| Vote date | 11-08-2026 |
| Rules | One idea per member; no idea discarded during generation; no evaluation until the round closed |

### 1.3 Solutions generated
 
Six ideas from six members, one each:
 
| # | Solution idea | Proposed by | Description | What the MS2 research showed about it |
|---|---------------|-------------|-------------|----------------------------------------|
| 1 | **Wishlist + price alerts** | Santiago Casasbuenas | A centralized app to save products from any store or social network into organized lists, keeping name, image, price, link and personal notes together, with price tracking and target-price alerts. | Problem 1. Interviews 1 (Emilio), 2 (Catherine), 3 (Cristian) and 6 (Laura & Mariana) — 5 of the 8 people interviewed. Journey Map 2 (Nico Alvarez). |
| 2 | **Hiking altitude tracker** | Jeronimo Franco | A route tracker that shows progress in terms of elevation and remaining effort instead of linear distance, applicable to hiking and cycling. | Problem 2. Interview 4 (Ari Sabogal), situations 1–4: estimating remaining difficulty from elevation, adapting pace to upcoming steep sections. |
| 3 | **Festival friend-finder** | Martin Riveira | A tool to locate members of a group inside a crowded event when mobile connectivity fails, offered as a shared platform rather than a per-event app. | Problem 3. Interview 5 (Gabriela Arrieta), situations 2 and 4: calls, WhatsApp and Instagram all failed; the fixed meeting point was not enough. |
| 4 | **School-bus tracking** | Juliana Durán | Real-time location and estimated arrival of the school bus for parents, with notifications when the child boards and gets off; extensible to pet transport services. | Problem 4. Interview 7 (Alfonso Durán), situations 1–4: waiting without information, calling the transport company, needing restricted access for safety. |
| 5 | **Campus parking availability** | Miguel Angel Velandia | Real-time availability, queue length and estimated waiting time for the parking lots near the university. | Not carried into MS2-O1: the course brief allowed only four problem statements, and this idea did not make the cut. It was never tested with a user. |
| 6 | **Grade calculator** | Juan Felipe Sáenz | A calculator to project final grades and required scores per course. | Not carried into MS2-O1: the course brief allowed only four problem statements, and this idea did not make the cut. It was never tested with a user. |
 
Only four problem statements could be carried into MS2-O1, so the four best-supported ideas went forward and were each taken to at least one interview. Ideas 5 and 6 were left out of that selection and were never tested with a prospective user, so they rest on the team's own assumptions alone.


### 1.4 Feature set derived from the MS2 evidence

Once the wishlist idea was selected, the team went back over the 28 What–How–Why situations and the two journey maps and asked, for each one, "what would have removed this friction?". This is not a second brainstorming session but an evidence-mapping exercise: every feature below is traceable to a specific situation, so the scope of the application is justified by user research rather than by preference.

| # | Feature idea | Situation it answers |
|---|--------------|----------------------|
| 1 | Save a product from any app through the system share sheet, without copying links manually | Int. 6, S4 — Mariana wants to export a product directly from Instagram instead of copying link, image and information by hand |
| 2 | Automatic capture of name, image, price and store when a link is pasted | Int. 3, S1 — Cristian pastes bare URLs into his own WhatsApp chat and cannot tell what a link is until he opens it |
| 3 | Target-price alert ("notify me when it drops below X") | Int. 3, S2 — he checks links manually every one or two weeks and misses offers; Int. 1, S3 — Emilio outsources price tracking to retargeted ads |
| 4 | Multiple lists by category (clothes, tech, gifts, travel) | Int. 1, S4 and Int. 2, S4 — validated as useful, but with an explicit warning about clutter |
| 5 | Per-item privacy instead of per-list privacy | Int. 2, S4 — Catherine wants to choose which individual items can be shared; Int. 3, S3 — Cristian rejects any social sharing entirely |
| 6 | Personal note field recording *why* the item was wanted | Int. 3, S4 — he wants to validate whether the desire persists after a few days and control impulse buying |
| 7 | Image-first grid view of saved items | Int. 6, S4 — Laura remembers products by seeing them; Int. 2, S3 — Catherine shops visually |
| 8 | Price comparison across stores, sorted from lowest to highest | Int. 2, S3 — Catherine explicitly asked for images, sources and prices ordered by price |
| 9 | Price history chart per product | Int. 3, S2 — deciding whether the current price is actually a good deal |
| 10 | Minimal, low-noise interface with no feed and no unnecessary features | Int. 1, S4 — Emilio fears the app becomes a graveyard of unused entries; Int. 2, S4 — Catherine insists on simplicity |
| 11 | Duplicate detection when the same product is saved twice from different sources | Int. 6, S1 — products end up scattered across screenshots, saved posts and tabs |
| 12 | Reminder of stale items ("you saved this 30 days ago — still interested?") | Int. 1, S2 — items he judged "not that important" simply fade from memory |

### 1.5 Smart features

The course requires the solution to include intelligent behaviour rather than plain CRUD. The team identified where machine learning, sensors and context can be applied, always tied to a real friction found in the interviews:

| Smart feature | How it works | Why it matters (evidence) |
|---------------|--------------|---------------------------|
| **Product recognition from a screenshot** | On-device OCR plus image recognition extracts the product name and store from a screenshot in the gallery and turns it into a structured entry. | Catherine and Laura both save products as screenshots (Int. 2 S2; Int. 6 S1). This meets users where they already are instead of asking them to change habit. |
| **Automatic categorization** | A text classifier assigns a saved product to a list (clothes / tech / gifts / travel) from its title and store. | Feature 4 was validated but users doubt they will maintain lists manually (Int. 1 S4). Automating it removes the maintenance cost. |
| **Best-time-to-buy prediction** | A model over the collected price history estimates whether the current price is near its historical minimum and suggests a target price. | Cristian tracks prices manually and still misses drops (Int. 3 S2); Emilio has no method at all (Int. 1 S3). |
| **Purchase-intent scoring** | The app ranks saved items by the likelihood the user still wants them, using recency, revisits, price movement and the personal note. | Directly answers Emilio's objection that lists fill up and are never acted on (Int. 1 S4). |
| **Context-aware notifications** | Alerts are batched and delivered when the user is likely to act (connectivity available, not in class hours), instead of firing on every price change. | Both Emilio and Catherine describe being overwhelmed by information (Int. 1 S4; Int. 2 S4). |
| **Eventual connectivity handling** | Local cache of the wishlist so items can be saved and consulted offline, syncing when the connection returns. | Course requirement; also observed in Int. 5, where connectivity failed exactly when it was needed. |

### 1.6 Evidence
Brainstorm: \
<img width="622" height="375" alt="image" src="https://github.com/user-attachments/assets/70a0eaf2-72a9-4837-a485-b17bd16e74a2" />


---

## 2. Idea Selection (Convergence Process)

> Explain the decision process based on what you have learned to select one idea (i.e., convergence and divergence strategies). Include the process used to select the idea for the semester, making it clear that a technique taught in class was used.

### 2.1 Divergence
 
The divergence phase deliberately kept the space open for as long as possible, and the narrowing happened in stages rather than in one decision:
 
1. **Six candidate solutions** were generated on the Miro board, one proposed by each member (Section 1.3).
2. **Four problem statements** were carried into MS2-O1 — the maximum the course brief allowed — covering unrelated domains: online shopping, hiking, large events and school transport.
3. **Seven interviews with eight participants** were conducted across those four problems, so that none of them was discarded before hearing a real user. Four of the seven were assigned to the leading idea, on the reasoning that the option most likely to be built deserved the deepest understanding.
4. **Twenty-eight situations** were derived using the **What–How–Why** technique, one set of four per interview, to move from what people said to why they behave that way.
5. **Two journey maps** were built for the most promising domain, exposing the moments of highest friction.
Concentrating the research on the leading idea carries an obvious risk of confirmation bias. The team accepted it deliberately, on the grounds that the alternative — spreading seven interviews evenly and understanding none of the four problems well — would have been worse for a one-semester project. The interviews were still run with open questions about current behaviour rather than about the proposed solution, and they did surface objections to the wishlist idea (Section 2.3).


### 2.2 Convergence
 
Two techniques taught in class were applied in sequence.
 
**Step 1 — Vote in the team chat (approval voting).** The consolidated list of six ideas was posted as a poll in the group chat, where each member could approve every idea they considered viable, not just one. Approval voting was chosen because it makes every member's preference visible with equal weight, avoids the loudest-voice effect of an open discussion, and shows not only the winner but how much support each alternative retained. Holding it the day after the board session rather than during it also gave everyone time to consider the ideas individually before committing.
 
This vote came before the user research, not after it. Its purpose was not to settle the semester's project but to rank the field: it decided which ideas were worth the cost of interviewing, and how the seven interviews should be distributed. The evidence gathered afterwards is what confirmed the result (Section 2.3).
 
| Idea | Approvals (out of 6) |
|------|----------------------|
| **Wishlist + price alerts** | **6 — unanimous** |
| Festival friend-finder | 5 |
| Hiking altitude tracker | 4 |
| Grade calculator | 2 |
| School-bus tracking | 2 |
| Campus parking availability | 0 |
 
The wishlist was the only idea approved by the entire team, and campus parking was the only one with no support at all. The four ideas that cleared the bar — wishlist, festival friend-finder, hiking and school-bus tracking — became the four problem statements carried into MS2-O1.

Votes: \
<img width="660" height="401" alt="image" src="https://github.com/user-attachments/assets/9baa0a1a-8415-46a2-be2f-ca1596b712b0" />

**Step 2 — Impact vs. Effort matrix.** A vote records *what* the team preferred but not *why*, so the result was validated against a 2×2 Impact vs. Effort matrix. Each member scored every idea from 1 to 5 on both axes and the team discussed the outliers until reaching a consensus score. This step also served as a check on the vote: had the matrix contradicted it, the team would have reopened the discussion.
 
- **Impact** = strength of the evidence gathered in MS2 (how many interviewees reported the pain, and how severe it was) plus the value the solution would add over the user's current workaround.
- **Effort** = technical complexity, availability of the data the solution depends on, external dependencies, and whether the scope fits four sprints.
  
| Idea | Impact (1–5) | Effort (1–5) | Quadrant | Reasoning |
|------|--------------|--------------|----------|-----------|
| Wishlist + price alerts | 5 | 2.5 | **Quick win** | Reported by 5 of the 8 interviewees, all with fragile workarounds. No external dependency: data comes from public product pages and from the user. Room for real smart features. |
| School-bus tracking | 4.3 | 4.4 | Major project | Strong emotional impact, but requires an agreement with a school or transport company, hardware on the vehicle, and handling location data of minors. |
| Hiking altitude tracker | 4 | 3.5 | Major project | Clear unmet need, but depends on accurate elevation data, GPS in areas with no coverage, and ideally wearable integration. |
| Festival friend-finder | 3.8 | 5 | Major project | The core requirement is to work *without* connectivity, which forces BLE/mesh or offline-first positioning — the highest technical risk of the set. |
| Campus parking availability | 3 | 3.8 | Money pit | Depends on sensor or institutional data the team does not have access to; without it the app relies on unverifiable user reports. |
| Grade calculator | 2 | 1.5 | Fill-in | Cheap to build, but no interview evidence, several existing alternatives, and almost no space for smart features. |

<img width="1582" height="1082" alt="image" src="https://github.com/user-attachments/assets/8676b159-229c-49f3-b339-1538f5e4ad69" />


### 2.3 Idea selected for the semester
 
**WhyNot — a centralized wishlist with price tracking and target-price alerts.**
 
The decision rests on four arguments:
 
1. **Evidence.** The vote pointed at the wishlist, and the research that followed did not contradict it: five of the eight participants described the same pain with independent workarounds (Amazon wishlist, Instagram saved posts, screenshots, browser tabs, self-messaging on WhatsApp, Steam wishlist), and it was the only problem for which several unrelated people reported the same friction. Had the interviews come back flat, the team would have gone back to the second-ranked idea.
2. **Feasibility within four sprints.** It is the only high-impact idea with no external dependency — no institutional agreement, no hardware, no connectivity guarantees in hostile environments.
3. **Room for intelligence.** The problem naturally supports the smart features listed in Section 1.5, whereas the grade calculator (the other low-effort option) does not.
4. **Prior validation.** A low-fidelity prototype was already built and presented in MS2, confirming that the main flow is understandable.

The main risk identified during convergence is **adoption**: Emilio explicitly doubted he would use an organized wishlist, and Catherine warned that the app must not add friction. The team therefore treats "saving a product must take fewer steps than a screenshot" as a design constraint for the whole semester, and prioritizes the smart capture features (screenshot recognition, share-sheet import, automatic categorization) over social or secondary functionality.

---


## 3. Empathy Maps

> Teams of 6 must submit **at least 5 empathy maps**, one per prospective user. Each empathy map should answer the Thinks / Sees / Feels / Does categories in relation to the interview evidence gathered in MS2.

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
<img width="818" height="742" alt="image" src="https://github.com/user-attachments/assets/588a1ca9-bcc0-4551-8781-f5a85b9473dc" />


---

## 4. Personas

> Teams of 6 must submit **at least 3 personas**. Each persona uses the layout from `MS3/resources/Persona Template.html` (Basic Info, Demographics, Goals, Pain Points, Environment). The table below links each persona's rendered HTML page — since GitHub only shows raw source for `.html` files, the "Live Preview" column wraps the source link with [htmlpreview.github.io](https://htmlpreview.github.io/) so it renders live in the browser.

| # | Persona | Image | Description | Source (repo) | Live Preview | Done By |
|---|---------|-------|-------------|---------------|--------------|---------|
| 1 | Emilio | <img src="personas/Emilio.jpeg" width="160"> | 23-year-old student at Universidad de los Andes; shops mainly for books and clothes, tracks items only via an Amazon wishlist | [emilio-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/emilio-persona.html) | [View live](https://raw.githack.com/Moviles-G13-S1/wiki/main/sprint_1/MS3/personas/emilio-persona.html) | Santiago Casasbuenas |
| 2 | Carlos | <img src="personas/Carlos.jpeg" width="160"> | Carlos is a practical, budget-conscious online shopper who carefully compares prices, reviews, and product quality before making confident purchasing decisions. | [carlos-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/carlos-persona.html) | [View live](https://htmlpreview.github.io/?https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/carlos-persona.html) | Jeronimo Franco |
| 3 | Andrea | <img src="personas/Andrea.jpeg" width="160"> | Andrea is an independent young woman who already works and lives alone. She enjoys shopping online more than in person, and she enjoys saving money on new items she hadn't noticed before. | [andrea-persona.html](https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/persona-andrea.html) | [View live](https://htmlpreview.github.io/?https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/persona-andrea.html) | Martin Riveira |

**How to add a new persona:**
1. Create the persona HTML file following the `MS3/resources/Persona Template.html` layout and commit it under `sprint_1/MS3/personas/`.
2. Copy its GitHub blob URL, e.g. `https://github.com/Moviles-G13-S1/wiki/blob/main/sprint_1/MS3/personas/<file-name>.html`.
3. Wrap it with the htmlpreview prefix to get the live preview link: `https://htmlpreview.github.io/?<paste the blob URL here>`.
4. Add a new row to the table above with the persona's name, a short description, the source link, and the wrapped preview link.

---

## 5. Solution Description

Our proposed solution is WhyNot, a mobile application designed to help users save, organize, compare, and keep track of products they are interested in buying. The solution addresses a common problem identified during our research: people frequently discover products across different online stores and social media platforms but are not always ready to purchase them immediately. As a result, products often end up scattered across screenshots, browser tabs, shopping carts, saved posts, notes, and wishlists from different platforms, making them difficult to find and compare later.

WhyNot provides users with one centralized place for everything they may want to buy. When users find a product they like, they can save it with relevant information such as its name, image, price, store, link, and category. Products can then be organized into personalized wishlists, allowing users to easily return to them and compare different alternatives instead of having to remember where each product was originally found.

The application also helps users decide when to buy, not only what to buy. WhyNot can track the prices of saved products and notify users when an item decreases in price, goes on sale, or reaches a target price previously selected by the user. This reduces the need to repeatedly visit different websites to check for discounts and can help users make more informed purchasing decisions.

The solution is designed around the different behaviors and needs identified in our user personas, including Emilio, Cristian, and Violeta. While they have different shopping habits and priorities, they share difficulties related to keeping track of products, comparing alternatives, remembering items they previously discovered, or knowing when it is a good moment to make a purchase. WhyNot brings these activities together while still allowing each user to organize and use the application according to their own shopping habits.

Overall, WhyNot aims to make the process between discovering a product and deciding to purchase it more organized, convenient, and informed. Rather than functioning as another online store, it acts as a personal shopping companion that connects products from different platforms and helps users manage the things they are considering buying.

---

## References

- Lim, Y. K., Stolterman, E., & Tenenberg, J. (2008). *The Anatomy of Prototypes.* ACM TOCHI, 15(2), 1–27. https://doi.org/10.1145/1375761.1375762
- Qualaroo — [Customer Journey Map guide](https://qualaroo.com/customer-journey-map/)
