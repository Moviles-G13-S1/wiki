# MS6 – Value Proposition & UI/UX Design

Team: #13

Members: Juliana Duran 202220671, Santiago Casasbuenas 202214932, Martin Riveira 202321727, Jeronimo Franco 202222204, Juan Felipe Saenz 202311148, Miguel Angel Velandia 202312487.

**Deadline:** September 12th, 5:00 a.m. (GMT-5) · **Deliverable:** MS6 wiki page link · **Possible points:** 10

---

MS6 (Week 6) goes deeper on the single solution the team selected — WhyNot — and locks down its visual identity. The deliverable defines the value proposition and the UI/UX design system (colour palette, typography, icons and images, UI prototype, and navigational patterns) that will carry into MS7 and into the GUI of the full application.

**Interactive prototype:** <https://why-not-wish-shop.lovable.app>

---

## 1. Value Proposition

**Owner**: Martin Riveira

**Problem addressed:**  
Users often find products they are interested in across different stores and platforms, but they are not always ready to buy them immediately. These products usually end up spread across screenshots, saved posts, browser tabs, notes, and store-specific wishlists, making them harder to organize, compare, and find again.

**Value delivered to users:**  
WhyNot gives users one place to save and organize products from different sources. Users can create wishlists, keep relevant product information together, compare alternatives, and track price changes without having to constantly check multiple platforms.

**Differentiation from existing solutions:**

| Existing alternative | What it does today | What WhyNot does differently |
| --- | --- | --- |
| Store-specific wishlists | Let users save products, but usually only within one store or platform. | WhyNot allows users to organize products from different stores and platforms in the same place. |
| Screenshots / saved posts | Help users remember products, but the information is unstructured and spread across different apps. | WhyNot stores products in an organized format with information such as image, price, store, and link. |
| Browser bookmarks and tabs | Save product links, but provide little organization and can become difficult to manage. | WhyNot turns saved products into organized wishlist items that can also be compared and tracked. |

**Main differentiating factor:**  
WhyNot combines products from different stores and platforms into one organized space, adding wishlist management, product comparison, and price tracking instead of limiting the user to a single store.

---

## 2. UI/UX Design

> Define important aspects of the UI/UX design: (i) colour palette and its rationale; (ii) fonts; (iii) icons and images; (iv) UI prototype; (v) navigational patterns. *(Max 10 points.)*

### 2.1 Colour Palette

**Owner:** *(TBD)*

| Role | Colour | HEX | RGB | Where it is used |
|------|--------|-----|-----|------------------|
| Primary | White | #FEFEFD | 254, 254, 253 | Main application colour and dominant visual base across the interface |
| Secondary | Beige | #EDE4D7 | 237, 228, 215 | Wishlist cards, product cards, image placeholders and highlighted content areas |
| Accent | Black | #171513 | 23, 21, 19 | Main action elements, headings, important labels and high-emphasis controls |
| Background | White | #FEFEFD | 254, 254, 253 | Main screen background throughout the application |
| Surface | Light Cream | #F5F1E9 | 245, 241, 233 | Form sections, grouped content areas and secondary containers |
| Text (primary) | Black | #171513 | 23, 21, 19 | Titles, headings, wishlist names, product names and important information |
| Text (secondary) | Grey | #817D78 | 129, 125, 120 | Subtitles, descriptions, navigation labels, prices and secondary information |
| Success / price drop | *(TBD)* | *(TBD)* | *(TBD)* | Price reductions, successful actions and positive status indicators |
| Warning / error | *(TBD)* | *(TBD)* | *(TBD)* | Errors, warnings and invalid input states |

**Rationale:**  
The colour palette was designed to give WhyNot a clean, calm, and minimal visual identity. The dominant white background keeps the interface simple and helps users focus on their saved products without unnecessary visual distractions. Beige and cream tones are used for cards, product placeholders, and grouped content, creating a warm and organized appearance that supports the idea of collecting and managing personal wishlists. Dark tones are reserved for important text and high-emphasis elements, while grey is used for secondary information. Overall, the palette reinforces WhyNot's purpose of making product saving, organizing, and tracking feel simple, personal, and visually consistent.

**Contrast and readability:**  
Contrast was checked between the main text colours and the backgrounds used throughout the interface. Primary text (#171513) provides a contrast ratio of approximately **18.05:1** on the main white background (#FEFEFD), **16.17:1** on the light cream surface (#F5F1E9), and **14.46:1** on the beige surface (#EDE4D7), comfortably meeting WCAG accessibility recommendations for normal and large text. Secondary grey text (#817D78) provides approximately **4.05:1** contrast on white, so it is best suited for larger or secondary text rather than small essential content. Its contrast is lower on cream and beige surfaces, so primary dark text should be preferred in those areas when readability is important.

**Palette image:**

<p>
  <img width="80" height="323" alt="Colour palette" src="https://github.com/user-attachments/assets/4e2efbfd-2430-4b9c-8b9c-26eb358c7298" />
</p>
---

### 2.2 Fonts

**Owner:** *(TBD)*

| Use | Typeface | Weight | Size | Notes |
|-----|----------|--------|------|-------|
| Titles / H1 | Poppins | Regular | 20 px | Used for main screen titles and section headings |
| Subtitles / H2–H3 | Poppins | Light | 15 px | Used for subtitles, supporting headings and secondary information |
| Body text | Frank Ruhl Libre | Regular | 15–20 px | Used for general content, names, product information and descriptive text |
| Buttons / labels | Poppins | Light / Regular | 15 px | Used for buttons, navigation labels, form labels and interactive elements |
| Captions / metadata | Poppins | Light | 15 px | Used for secondary information such as item counts, prices, hints and small descriptions |

**Rationale:**  
The typography combines Poppins and Frank Ruhl Libre to create a balance between clarity and personality. Poppins is used for interface-oriented elements such as titles, subtitles, labels, and navigation because its clean geometric shapes are highly legible on mobile screens. Frank Ruhl Libre is used for selected body text and prominent content, adding a more distinctive and editorial character to the interface. Together, both typefaces support readability while giving WhyNot a minimal, elegant, and recognizable visual identity.

**Consistency:**  
The type scale is applied consistently across all screens to maintain a clear visual hierarchy. Main titles use Poppins Regular at 20 px, while subtitles and secondary information use Poppins Light at 15 px. Frank Ruhl Libre is used mainly for body content and selected prominent text at 15 px or 20 px depending on its importance. The same font sizes and weights are reused for equivalent elements across screens, helping users quickly recognize headings, supporting information, labels, and content.



---

### 2.3 Icons and Images

**Owner:** *(TBD)*

**Icon style:** *(TBD — e.g. outlined, filled, rounded; icon set or library used; stroke weight and grid size.)*

| Icon | Meaning | Where it is used |
|------|---------|------------------|
| *(TBD)* | *(TBD)* | *(TBD)* |
| *(TBD)* | *(TBD)* | *(TBD)* |
| *(TBD)* | *(TBD)* | *(TBD)* |
| *(TBD)* | *(TBD)* | *(TBD)* |
| *(TBD)* | *(TBD)* | *(TBD)* |

**Image style:** *(TBD — how product images, empty states, and illustrations are treated: aspect ratios, corner radius, placeholders, image-first cards.)*

**Visual consistency:** *(TBD — the rules that keep icons and imagery coherent across the app.)*

*(Insert the icon sheet and image-style examples here — high resolution and legible.)*

---

### 2.4 UI Prototype

**Owner:** Juliana Duran (group 13)

**Design tool used:** figma

**Interactive prototype link for editting:** <https://www.figma.com/design/GKjDHU7klmjGONACLHfg0O/WhyNot-IOS?node-id=0-1&t=qpzvDMk08xzDNPHs-1>

**Interactive prototype link for preview (ui version):** <https://www.figma.com/proto/GKjDHU7klmjGONACLHfg0O/WhyNot-IOS?node-id=30-367&p=f&t=se9HfCJDNc6lyavh-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=30%3A367>

**Main screens included:**
### User UI

| # | Screen | Purpose | Key interactions shown |
|---|---|---|---|
| 1 | [Login](ui-prototype/user/Login.png) | Allows existing users to access their WhyNot account. | Enter email and password, log in, or navigate to account creation. |
| 2 | [Create an Account](ui-prototype/user/CreateAccount.png) | Allows new users to register in WhyNot. | Enter personal information, password, and preferred category. |
| 3 | [Home](ui-prototype/user/Home1.png) | Provides a personalized overview of the user's shopping activity. | Search products, access wishlists, view nearby items, and see recommendations. |
| 4 | [My Wishlists](ui-prototype/user/MyWishlists.png) | Organizes saved products into different categories. | Browse existing wishlists and create a new wishlist. |
| 5 | [New Wishlist](ui-prototype/user/NewWishlist.png) | Allows users to create a new wishlist. | Select a category, upload a picture, save, or cancel. |
| 6 | [Wishlist Detail](ui-prototype/user/WishlistDetail.png) | Displays products saved within a specific wishlist. | Browse products, add items, and apply filters. |
| 7 | [Save Product Automatically](ui-prototype/user/SaveProductAutomatically.png) | Allows users to save a product using its link. | Paste a product link, select a wishlist, and save the item. |
| 8 | [Save Product Manually](ui-prototype/user/SaveProductManually.png) | Allows users to manually add a product. | Enter product information, upload an image, select a wishlist, and save. |
| 9 | [Product Detail](ui-prototype/user/ProductDetail.png) | Displays detailed information about a saved product. | View prices, edit the item, and mark it as purchased. |
| 10 | [Purchases](ui-prototype/user/Purchases.png) | Keeps a record of purchased products. | Browse and filter purchased products. |
| 11 | [Profile](ui-prototype/user/Profile.png) | Displays the user's personal information and preferences. | View account information and access profile editing. |
| 12 | [Edit Profile](ui-prototype/user/EditProfile.png) | Allows users to update their personal information. | Edit profile information and access password settings. |
| 13 | [Change Password](ui-prototype/user/ChangePassword.png) | Allows users to update their password. | Enter the current and new password and save the changes. |

### Administrator UI

| # | Screen | Purpose | Key interactions shown |
|---|---|---|---|
| 1 | [Saved Products per User](ui-prototype/admin/SavedProducts%users.png) | Shows the number of products saved by users. | Analyze saved-product activity per user. |
| 2 | [Saved Products — Users](ui-prototype/admin/SavedProductsUsers.png) | Provides a detailed user-level view of saved products. | View and compare individual users. |
| 3 | [Save Methods](ui-prototype/admin/SavedMethods.png) | Shows how users save products in WhyNot. | Compare the different product-saving methods. |
| 4 | [Sidebar](ui-prototype/admin/Sidebar.png) | Displays the administrator navigation menu. | Navigate between the different analytics views. |
| 5 | [Purchased Products](ui-prototype/admin/PurchasedProducts.png) | Shows information about purchased products. | Analyze purchasing activity and product data. |
| 6 | [Demographic Profile](ui-prototype/admin/DemographicProfile.png) | Shows demographic information about WhyNot users. | Analyze demographic characteristics and distributions. |

**How the prototype reflects the design system:** *(TBD — point to where the palette, typography, icons, and image style from sections 2.1–2.3 appear in the screens above.)*

---

### 2.5 Navigational Patterns

**Owner:** *(TBD)*

## 2.5 Navigational Patterns

**Owner:** TBD

**Main navigation pattern:**  
Bottom navigation bar with four top-level destinations: Home, Wishlists, Purchases, and Profile. More specific screens use hierarchical navigation from these main sections.

**Navigation components used:**

| Component | Used for | Screens involved |
| --- | --- | --- |
| Bottom navigation bar | Moving between the main sections of the app | Home, Wishlists, Purchases, Profile |
| Back navigation | Returning to the previous screen after entering a more specific section | Wishlist Detail, Product Detail, New Wishlist, Save Product, Edit Profile, Change Password |
| Cards / list items as entry points | Opening wishlists, products, and other detailed information | Home, Wishlists, Wishlist Detail, Purchases |
| Action buttons | Starting actions such as creating a wishlist, adding a product, editing information, or saving changes | Wishlists, Wishlist Detail, Product Detail, Profile |
| Sidebar navigation | Moving between the different analytics views available to administrators | Administrator analytics screens |

**Why this pattern fits WhyNot:**  
WhyNot has a small number of main sections that users need to access frequently, so a bottom navigation bar keeps these destinations visible and easy to reach. More specific actions are placed inside their corresponding sections, which keeps the main navigation simple and avoids unnecessary options. The administrator interface uses a sidebar instead because administrators mainly move between different analytics views.

**Navigation flow:**
<img width="1448" height="1086" alt="image" src="https://github.com/user-attachments/assets/ffa574d4-630e-49c5-9a64-b3fb3c52adfb" />


---

## 3. Submission Notes

- The graded artifact is the **MS6 wiki page**; the link is submitted through Bloque Neón before the deadline.
- GitHub records edit timestamps in **GMT (UTC+0)** while the deadline is in **GMT-5**. The page must not be edited after September 12th, 5:00 a.m. (GMT-5) — later edits result in a grade of 0.
- Per the course GenAI guidelines, AI may be used for brainstorming and outlining only; no AI-generated content may appear in the final submission. For prototyping and visual design, AI use is permitted at level 4 of the AI Assessment Scale.
- Progress against the official requirements is tracked in [MS6_Deliverable_Checklist.md](./MS6_Deliverable_Checklist.md).

---

## References

- Chapter 6 of the course book — *(add link)*
- Chapter 7 of the course book — architecture styles and patterns — *(add link)*
- Perkins, M., Furze, L., Roe, J., & MacVaugh, J. (2023). *The AI Assessment Scale (AIAS): A Framework for Ethical Integration of Generative AI in Educational Assessment.*
- Lim, Y. K., Stolterman, E., & Tenenberg, J. (2008). *The Anatomy of Prototypes.* ACM TOCHI, 15(2), 1–27. https://doi.org/10.1145/1375761.1375762
