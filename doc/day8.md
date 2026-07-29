Day 8 – Admin Product Routes (Create/Update/Delete)
Date: July 29, 2026
Module: 2 (July 27 – Aug 02, 2026)

- Objective
Complete the Product API by adding admin-level routes to create, update, 
and delete products.

- Work Completed

1. Product Controller (additions)
- Created `createProduct()` — adds a new product to MongoDB.
- Created `updateProduct()` — updates an existing product by ID.
- Created `deleteProduct()` — removes a product by ID.

2. Product Routes (additions)
- Added routes:
  - `POST /api/products` → create a new product
  - `PUT /api/products/:id` → update a product
  - `DELETE /api/products/:id` → delete a product

3. Testing
- Tested all three routes using Postman:
  - Created new sample products.
  - Updated fields (price, quantity) on an existing product.
  - Deleted a test product and confirmed it no longer appears in GET requests.
- Added basic validation (required fields must be present before creating 
  a product).

- Decisions Made
- Admin routes are open for now (no auth restriction) since the User/Auth 
  system is being built in Module 3 — will be protected with JWT middleware 
  once authentication is implemented.

## Next Steps (Day 11)
- Connect the Shop page (shop.html) to the live GET /api/products endpoint.
- Connect the Single Product page to GET /api/products/:id.
