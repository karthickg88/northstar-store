# Northstar E-commerce — Deployment Bundle

This is a static, browser-based storefront. It requires no build step, Node.js, or database.

## Deploy on Netlify
1. Open https://app.netlify.com/drop
2. Sign in if prompted.
3. Drag the entire `northstar-deploy` folder (or upload a ZIP containing its contents) into the drop area.
4. Netlify will provide a public URL after deployment.

## Deploy on Vercel
1. Create a new project at https://vercel.com/new and import a Git repository containing these files, or install the Vercel CLI.
2. Set the project root to the folder containing `index.html`.
3. Choose the Other/framework preset and leave build command and output directory empty (or use `.` as the output directory if required by the dashboard).
4. Deploy.

## Deploy on GitHub Pages
1. Create a GitHub repository and upload `index.html` and `.nojekyll`.
2. In repository Settings → Pages, select deployment from the `main` branch and `/ (root)`.
3. Save and wait for the published URL.

## Important limitations
- This is a frontend demo, not a production commerce backend.
- Checkout is simulated; no payment is collected and no real order is created.
- Products are sample data in `index.html`.
- Wishlist and cart currently live in browser memory and reset when the page is refreshed.
- Newsletter signup does not submit email addresses to a mailing service.
- Before accepting real orders, add a secure backend/database, persistent carts and orders, server-side validation, privacy/returns policies, and a payment provider such as Razorpay. Never put secret API keys in frontend code.
