Banarasiya Silk Sarees & Craft — Static Website

This is a static, Netlify-ready website for a traditional Banarasi silk saree manufacturer.

Structure
- index.html — Home page
- products.html — Product grid and product cards
- product.html — Product detail template (reads product details from query string)
- contact.html — Contact info and Netlify order form
- css/style.css — Styles
- images/ — Sample placeholder images (SVG)

How to add or update products
- To add a product to the products grid, open `products.html` and copy one of the `<article class="product">` blocks.
- Update image path (in `src`), the product name inside the `<h4>`, the price, description, and the `href` on the main link.

Using the product detail template
- Product links point to `product.html` and pass data in the query string. Example:

  `product.html?name=Banarasiya%20Maroon%20Saree&price=9500&img=images/sample1.svg&category=Saree&desc=Handwoven%20gold-zari%20motifs`

- `product.html` reads these query params and displays the product. To create standalone product pages, duplicate `product.html` and change the static values.

WhatsApp ordering
- Buttons with "Order on WhatsApp" open WhatsApp web or the app with a pre-filled message. The phone numbers used are:
  - +91 8009854081
  - +91 8707457279

Netlify forms
- The contact/order form uses Netlify Forms (no backend required). Ensure when deploying to Netlify you allow forms in settings.
- The form name used is `order`. Netlify will capture submissions automatically.

Deploy on Netlify
1. Zip the `site` folder and drag-and-drop to Netlify Sites (Sites → Add new site → Deploy manually).
2. Or push this folder to a GitHub repository and connect the repository in Netlify. Set publish directory to `/` or to the folder that contains `index.html` depending on your repo root.

Notes & Customization
- Replace SVG placeholders in `images/` with real product photographs (same filenames or update the HTML).
- Colors are in `css/style.css` at `:root` variables. Change `--maroon`, `--gold`, and `--cream` to adjust the theme.
- Headings use `Playfair Display` from Google Fonts; body uses `Rubik`.

If you want, I can:
- Add product JSON and a small admin script for generating product cards.
- Create separate static product pages for each item.
- Connect a simple search/filter on `products.html`.
