Day 9 – Connecting Shop & Single Product Pages to Live Backend Data
Date: July 30, 2026
Module: 2, Day 4 (July 27 – Aug 02, 2026)

- Objective
Replace the static, hardcoded product listings on the Shop and Single
Product pages with real data fetched live from the backend API built in
Days 8–10.

- Work Completed

1. Shop Page (shop.html)
- Removed the hardcoded product cards from the page markup.
- Replaced them with a single empty container (`#shop-products`) that
  JavaScript populates on page load.
- Added `loadShopProducts()` in `script.js`, which:
  - Calls `GET /api/products`.
  - Dynamically builds a product card (image, category, name, star rating,
    price) for each product returned.
  - Links each card to `sproduct.html?id=<productId>`.
  - Shows a friendly message if the backend isn't running or no products
    exist yet (e.g. "Run `node seed.js`...").

2. Single Product Page (sproduct.html)
- Replaced hardcoded product name/price/description/image with placeholder
  elements (`#pd-name`, `#pd-price`, `#pd-description`, `#pd-category`,
  `#MainImg`) that get filled in dynamically.
- Added `loadSingleProduct()` in `script.js`, which:
  - Reads the product ID from the URL query string (`?id=...`).
  - Calls `GET /api/products/:id`.
  - Fills in the product details on the page.
  - Shows a clear message if no ID is passed, or if the product/backend
    isn't reachable.

3. Related Products
- Added `loadRelatedProducts()`, which fetches all products, filters out
  the current one, prioritizes items from the same category, and displays
  up to 4 related product cards below the main product.

4. Shared Rendering Logic
- Added a shared `buildProductCard()` helper in `script.js` so the Shop
  page and the Related Products section use identical, consistent card
  markup instead of duplicated code.

5. Error Handling
- Both pages now handle three states gracefully: loading, successfully
  loaded data, and failure (backend not running / network error) — instead
  of showing blank or broken content.

- Decisions Made
- API base URL is defined once as a constant (`API_BASE_URL` in
  `script.js`) for easy updating later (e.g. when a real deployment URL
  is needed, even though this project stays local for now).
- "Add to Cart" buttons remain visually present but non-functional — real
  cart logic is scoped for Module 3, not this module.

Next Steps (Module 3 – Aug 03 – Aug 09, 2026)
- Implement Cart schema/API and connect it to the Cart page.
- Implement Signup/Login with JWT.
- Connect the Contact form to a backend endpoint.
