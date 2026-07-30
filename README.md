# Ecommerce-management-System
This web is a full-stack, responsive e-commerce web application built with  HTML5, CSS3, JavaScript, and Tailwind CSS on the frontend, and Node.js,  Express.js, and MongoDB (local instance) on the backend. This is a local  development project and is not deployed to a live server.
## Progress Log

### Day 1 – July 20, 2026
- Conducted requirement gathering and finalized the overall project scope.
- Sketched wireframes for the core pages: Home, Shop, Product Details, 
  Cart, Signup/Login, and Contact.
- Outlined the main user flow: browsing products → viewing product details 
  → adding to cart → signing up/logging in → checkout → contact support.
- Further description added in docs/day1.md

### Day 2 – July 21, 2026
- Finalized wireframes and confirmed the page structure based on Day 1 sketches.
- Planned the project folder architecture:
  - `client/` – frontend (HTML, CSS, JS, Tailwind)
  - `server/` – backend (Node.js, Express, MongoDB models/routes)
- Decided on naming conventions and basic project structure for both folders.
- Further description added in docs/day1.md

### Day 3 – July 22, 2026
- Created the GitHub repository and set up the base folder structure (client/, server/, docs/).
- Initialized the frontend with Tailwind CSS and the backend with Express.
- Built the responsive Homepage (navbar, hero section, featured products, footer).
- Further description added in docs/day3.md.

### Day 4 – July 23, 2026
- Built the Cart page with item list, quantity controls, and order summary.
- Built the About page with store introduction and mission statement.
- Built the Contact Us page with form fields and contact info section.
- Further description added in docs/day4.md.

### Day 5 – July 24, 2026
- Built the responsive Shop page with a product grid layout (image, name, price).
- Built the Single Product page with detailed view and "Add to Cart" button.
- Built the Signup/Login page with toggle between the two forms.
- Further description added in docs/day5.md.

### Day 6 – July 27, 2026
- Designed the MongoDB Product schema using Mongoose with product fields (name, description, price, quantity, image, category).
- Connected the Product model to the Express backend and tested it with sample data in MongoDB Compass.
- Organized the backend structure by preparing the models, routes, and controllers folders for the upcoming Product API.
- Further description added in docs/day6.md.
- <img width="317" height="310" alt="image" src="https://github.com/user-attachments/assets/25d3de13-f4d4-4505-b394-493a158af38e" />

### Day 7 – July 28, 2026
- Built the Product API with GET routes to fetch all products and individual product details from MongoDB.
- Created the product controller and connected the routes to the Express backend.
- Tested the API endpoints in Postman, including proper error handling for invalid product IDs.
- Further description added in docs/day7.md.

### Day 8 – July 29, 2026
- Completed the Product API by adding admin routes to create, update, and delete products in MongoDB.
- Implemented the corresponding controller functions and connected them to the Express backend routes.
- Tested all CRUD operations in Postman and added basic validation for required product fields.
- Further description added in docs/day8.md.

### Day 9 – July 30, 2026
- Connected the Shop page to the live GET /api/products endpoint — products now load dynamically instead of being hardcoded.
- Connected the Single Product page to GET /api/products/:id, reading the product ID from the URL.
- Added a shared product-card renderer used by both the Shop page and the Related Products section.
- Added error handling so both pages show a clear message if the backend isn't running instead of breaking.
- Further description added in docs/day9.md.

## Tech Stack
- Frontend: HTML5, CSS3, JavaScript (ES6+), Tailwind CSS
- Backend: Node.js, Express.js, MongoDB (local), Mongoose
- Tools: Git, GitHub, Postman, VS Code, MongoDB Compass
