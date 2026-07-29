Day 7 – Product API (GET Routes)
Date: July 28, 2026
Module: 2 (July 27 – Aug 02, 2026)

- Objective
Build and test the read-only Product API endpoints so the frontend can 
start fetching real product data.

- Work Completed

1. Product Controller (controllers/productController.js)
- Created `getAllProducts()` — fetches and returns all products from MongoDB.
- Created `getProductById()` — fetches a single product by its MongoDB ID.

2. Product Routes (routes/productRoutes.js)
- Set up routes:
  - `GET /api/products` → returns all products
  - `GET /api/products/:id` → returns a single product

3. Testing
- Tested both endpoints using Postman to confirm correct JSON responses.
- Verified error handling for an invalid/non-existent product ID 
  (returns a proper 404 response instead of crashing the server).

- Decisions Made
- API responses follow a consistent JSON format: `{ success: true, data: ... }`.
- Error responses also follow a consistent format: `{ success: false, message: ... }`.

- Next Steps (Day 10)
- Build admin routes (create/update/delete product).
- Begin connecting the Shop page to the live GET API.
