# Sprint 3 Roadmap — WhyNot (Team 13)

*Created: Oct 5, 2026 · Sources: Drive `Sprint 3/` (Sprint 3 Activity description, VivaVoce3 rubric, App Report 3) + repos `wiki`, `whynot-front-kotlin`, `whynot-front-flutter`, `whynot-back`.*

## 1. Key dates

| Date | What |
|---|---|
| Mon Oct 5 | Sprint 3 opens |
| Sat Oct 24, 23:59 | App Report 3 (optional, 75 individual pts, PDF in BN, cumulative parts 1–3) |
| **Sat Oct 31, 05:00** | **Sprint 3 deadline** — wiki + repos frozen (GitHub last-edit timestamp is checked), repo link in BN, APK/iOS shared within 10-min grace |
| After Oct 31 | Viva voce (110 individual pts) |

Internal target: **everything submitted Fri Oct 30 by 22:00** — never work against the 5 AM cutoff.

## 2. What is graded

**Team (180):** co-evaluation × repo multipliers (134) · ethics video, 6 min (46).
**Individual (165):** wiki (15 — eventual-connectivity scenarios) · viva voce (110) · process competences (40).

**Viva voce (per person, 110):**

| Item | Pts | How to max it (from VivaVoce3 rubric) |
|---|---|---|
| Justify the 4 strategies of teammates on *your* platform | 20 | Opens the exam: 1 min per column, technical vocabulary is graded |
| Own BQ | 10 | Data comes from the analytics engine (real-time or on-demand, never manual/downloaded files), in the pipeline, with UI. **One DB, one dashboard** |
| Multithreading | 20 | **Kotlin:** coroutine+dispatcher 5 · nested coroutines with IO 10 · one IO + one Main 10. **Flutter:** Future 5 · Future w/ handler 5 · handler + async/await 10 · Stream 5 · Isolate 10 |
| Local storage | 20 | Relational DB 10 · Key/value DB (Hive/Realm) 5 · Local files 5 · Preferences/DataStore/Keychain 5 |
| Eventual connectivity | 20 | 5 per protected view. **No generic app-wide "no connection" message** — each view needs its own navigation/offline behavior |
| Caching | 20 | Image-cache lib (Coil/Glide/CachedNetworkImage) 5 · LRU/SparseArray/ArrayMap/NSCache 10 (explain structure, parameters, decisions) |

Full points require **each member** to own code for every strategy — "1 per app" in the description is the minimum, not the target.

**Hard gates (deliverable not graded / not eligible for viva):** wiki item 3 (features, BQs, strategies list) · app runs on a real device · collaboration evidence (issues, milestones, board, PRs with review/approval, squash merges, verbose commits). Each bug the TAs find: **−0.3**.

## 3. Where we stand (repo audit, Oct 5)

- Sprint 2 features implemented on both apps; last merges Oct 2.
- **Open S2 gaps:** Flutter does not call `save_recommended_product`; physical-device demo evidence pending; merged PRs have **no formal reviews** (hurts the β multiplier); several generic commit messages ("error", "done runner").
- **Kotlin:** coroutines are only `viewModelScope.launch` (+2 `withContext`) — no explicit IO dispatchers, no Room, DataStore, Coil or LruCache, no connectivity monitoring.
- **Flutter:** `pubspec.yaml` has no local storage, image cache or connectivity packages; Futures/Streams exist but no Isolates.
- Firestore's built-in offline persistence is on by default but not configured or justified anywhere — it does not count as an EC strategy by itself.
- **BQs:** all 6 Sprint 1 BQs were used in Sprint 2. Sprint 3 needs **6 new ones** (one per member), drawn from the MS4 candidate list.

## 4. Proposed Sprint 3 BQs

| Owner | Platform | BQ | Type | Data needed (new) |
|---|---|---|---|---|
| Miguel | Kotlin | How much money have users saved on the products they marked as purchased? | 2 | `purchasePrice` captured at `markPurchased` vs saved `price` |
| Martin | Kotlin | How often do users manually add a product (vs. add-by-link)? | 3 | `source: manual \| link \| voice \| recommendation` on product create |
| Juan Felipe | Kotlin | Which features are less used? | 3 | `analyticsEvents` feature_open/feature_complete |
| Juliana | Flutter | How many clicks does it take a user to save a product? | 2 | funnel events per save session (start → save/abandon) |
| Jeronimo | Flutter | How many errors does the app produce weekly? | 1 | `appErrors` written by global error handlers (queued offline) |
| Santiago | Flutter | How many writes are made offline and how long until they sync? | 1 | `pendingSync` / `syncedAt` per queued write *(new BQ — not in MS4 list)* |

⚠️ Verify against the Sprint 1 per-type limits before committing. Events must be emitted by **both** apps into the same Firestore collections (single DB rule).

## 5. Strategy ownership (each member owns one vertical)

### Kotlin / Android
| Member | Vertical | Threading | Local storage | Caching | EC (protected views) |
|---|---|---|---|---|---|
| Miguel | Wishlists, products, purchases | Repos on `Dispatchers.IO`, result to Main; nested `async` for wishlist + products load | **Room** (offline products/wishlists, source of truth) | **Coil** for product images | Wishlists, Wishlist Detail, Product Detail, Purchases |
| Martin | Home, add product, nav | `withContext(IO)` for link parsing / save, UI on Main | **DataStore** (draft product form, last filters) | **LruCache** for Home sections | Home, New Product (offline save queue), Add by link (blocked w/ specific message), Nearby |
| Juan Felipe | Auth, profile, admin, recommendations | Nested coroutines for parallel admin queries (`coroutineScope { async… }`) | Local **file** (admin snapshot JSON) + DataStore session | **LruCache/ArrayMap** for recommendations & admin metrics | Login/Register, Profile/Edit, Admin dashboards, Recommendations |

### Flutter / iOS
| Member | Vertical | Threading | Local storage | Caching | EC (protected views) |
|---|---|---|---|---|---|
| Juliana | Products, wishlists, smart/nearby | Future w/ handler + async/await (save flows) | **sqflite/drift** relational offline store for products/wishlists | **cached_network_image** | Wishlists, Product Detail, New/Edit Product (offline queue), Recommendations |
| Jeronimo | Auth, profile, home | **Stream** (connectivity_plus) + async/await | **shared_preferences** + **flutter_secure_storage** (Keychain) | LRU cache for city catalog/profile | Login, Create Account, Profile, Home |
| Santiago | Admin + sync engine | **Isolate** (`compute`) for BQ aggregations over full collections | **Hive** (admin metrics snapshot, sync queue) | LRU map for admin metrics w/ TTL | All admin views (last-synced timestamp, stale banner) |

Each member must also be able to explain the other two members' columns on their platform (20 pts).

## 6. Weekly plan

**Week 1 · Oct 5–11 — Foundations**
- Sprint 3 milestone + GitHub Project board; one issue per member per strategy + BQ (≈30 issues). From now on: **PR + 1 reviewer approval + squash merge**, verbose commits.
- Backend (`whynot-back`): schema + rules for `analyticsEvents`, `appErrors`, `purchasePrice`, `source`.
- Add dependencies: Kotlin (Room, DataStore, Coil, connectivity `NetworkCallback` → Flow); Flutter (connectivity_plus, sqflite/drift, hive, shared_preferences, cached_network_image).
- Flutter: implement `save_recommended_product` (S2 carry-over).
- Wiki: draft the **EC scenarios** section (15 pts) — which scenarios, expected behavior per view.

**Week 2 · Oct 12–18 — Strategies**
- Each member implements local storage + threading + caching in their vertical.
- Both apps emit the new BQ events.
- Mid-sprint demo on a **real device** (Fri Oct 16).

**Week 3 · Oct 19–25 — BQs + EC everywhere**
- BQ views on the admin dashboard, fed live from Firestore.
- EC on **every** functionality (item 8): view-specific offline states, queued writes, retry.
- Ethics video: script + recording.
- App Report 3 (optional) — due Sat Oct 24.

**Week 4 · Oct 26–30 — Freeze & submit**
- Mon–Tue: bug bash on real devices, airplane-mode scenarios, screenshots/videos for the wiki.
- Wed Oct 28: code freeze.
- Thu Oct 29: Sprint 3 wiki page complete (features, BQs with owner/type/rationale, 4 strategy sections, EC evidence, contribution table, ethics video link).
- Fri Oct 30: APK via Firebase App Distribution to the 7 TAs + Teams message; iOS TA coordination; repo link in BN.
- Viva prep: each person gives a 4-minute walkthrough of their own and teammates' strategies.

## 7. Risks
- **BQ type limits** may block the proposed set — check this week.
- Room/drift as the offline source of truth means repository rewrites — start in week 1, not week 3.
- Missing PR reviews → zero multipliers → zero sprint grade. Enforce from day 1.
- Drive `Sprint 3` has no MS folders yet; adjust when weekly MS deliverables appear.