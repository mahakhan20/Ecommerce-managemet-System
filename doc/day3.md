Day 3 – Repository Setup & Project Initialization
Date: July 22, 2026
Module: 1 (July 20 – July 26, 2026)
- Objective
Set up the actual project repository and initialize both the frontend and 
backend so coding can begin from Day 4 onward.

- Work Completed

### 1. GitHub Repository Setup
- Created the ShopSphere repository on GitHub.
- Added a `.gitignore` file to exclude `node_modules/` and `.env`.
- Set up the base folder structure: `client/`, `server/`, `docs/`.

- 2. Frontend Initialization (client/)
- Created empty HTML files for all planned pages:
  `index.html`, `shop.html`, `product.html`, `cart.html`, `signup.html`, `contact.html`.
- Linked Tailwind CSS (via CDN for now) in each HTML file.
- Created `css/styles.css` for custom styles on top of Tailwind.
- Created placeholder JS files: `shop.js`, `product.js`, `cart.js`, `auth.js`, `contact.js`.

- 3. Backend Initialization (server/)
- Ran `npm init` to set up `package.json`.
- Installed Express: `npm install express`.
- Created `server.js` as the entry point with a basic Express app and a test route.
- Confirmed the server runs locally on a chosen port (e.g. `http://localhost:3000`).

- Decisions Made
- Server will run on port 5000; client will be opened separately (e.g. via 
  Live Server) during development.

## Next Steps (Day 4)
- Build the Homepage layout (navbar, hero section, featured products, footer).
- Test responsiveness across screen sizes.
