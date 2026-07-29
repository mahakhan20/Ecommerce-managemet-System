Day 6 – Product Schema Design
Date: July 27, 2026
Module: 2 (July 27 – Aug 02, 2026)

- Objective
Design the MongoDB Product schema and connect it into the Express backend, 
laying the foundation for the Product API.

- Work Completed

1. Product Schema (models/Product.js)
- Defined the Product schema using Mongoose with the following fields:
  - `name` (String, required)
  - `description` (String)
  - `price` (Number, required)
  - `quantity` (Number, required)
  - `image` (String — image URL/path)
  - `category` (String, optional)
  - `createdAt` (Date, default: now)

2. Model Testing
- Connected the schema to the local MongoDB database (already configured 
  in Module 1).
- Manually inserted a few sample products via MongoDB Compass to verify 
  the schema structure works correctly.

3. Folder Organization
- Confirmed `models/`, `routes/`, and `controllers/` folders are ready 
  for the upcoming Product API work.

- Decisions Made
- Kept the schema simple for now (no variants/sizes) to match project scope.
- Sample/dummy product data will be used for development and testing 
  before real content is added later.

## Next Steps (Day 9)
- Build REST API routes for products (GET all, GET single).
