Day 5 – Shop, Single Product & Signup Page Development
Date: July 24, 2026
Module: 1 (July 20 – July 26, 2026)

- Objective
Build the remaining core frontend pages — Shop, Single Product, and 
Signup/Login — completing the full set of static, responsive pages for 
ShopSphere before backend integration begins in Module 2.

- Work Completed

1. Shop Page (shop.html)
- Built the product listing layout showing all products in a grid 
  (image, name, price).
- Used a responsive grid: 1 column on mobile, 2 on tablet, 3–4 on desktop.
- Linked each product card to the Single Product page.
- Data is static/placeholder for now — will be connected to the Product 
  API in Module 2.

2. Single Product Page (sproduct.html)
- Built the product details layout: large product image, name, 
  description, price, quantity selector, and "Add to Cart" button.
- Made the layout responsive — image and details stack on mobile, 
  side-by-side on desktop.
- Static/placeholder data for now — will fetch real product data via API 
  in Module 2.

3. Signup/Login Page (signup.html)
- Built the signup form (Name, Email, Password) and login form 
  (Email, Password) with a toggle/link between the two.
- Kept the form centered and compact, resizing cleanly on mobile.
- Form is UI-only today — authentication logic (bcrypt, JWT) will be 
  added in Module 3.

4. Responsiveness Testing
- Tested all three pages across mobile, tablet, and desktop breakpoints.
- Fixed spacing and alignment issues found during testing.

## Decisions Made
- All static frontend pages are now complete: Home, Shop, Single Product, 
  Cart, Signup/Login, About, Contact.
- From Module 2 onward, focus shifts entirely to backend development 
  (Express + MongoDB) and connecting these pages to live APIs.

Next Steps (Module 2)
- Set up MongoDB schemas (Product, User).
- Build REST APIs for products.
- Connect Shop and Single Product pages to the backend.
