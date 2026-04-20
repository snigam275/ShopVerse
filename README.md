# ShopVerse - Responsive E-Commerce Website

A modern, responsive front-end e-commerce website built with plain HTML, CSS, and JavaScript.

This project includes a complete multi-page shopping flow with product browsing, filtering, product details, cart management, coupon discounts, dark mode, and persistent cart/theme state using localStorage.

## Live Features

- Responsive layout for desktop, tablet, and mobile
- Sticky navigation with mobile menu toggle
- Dark mode toggle with saved preference
- Product listing page with:
  - Search
  - Category filters
  - Price range filter
  - Rating filter
  - Sorting (price, rating, name)
  - Grid/List view toggle
- Dynamic product detail page based on URL query (`?id=`)
- Add to cart from listing and product detail pages
- Cart page with:
  - Quantity updates
  - Remove item
  - Clear cart
  - Coupon codes (`SAVE10`, `SHOP20`, `WELCOME15`)
  - Shipping, tax, discount, and total calculation
  - Mock checkout flow
- Toast notifications for user actions
- Scroll animations and interactive UI effects

## Project Structure

```
ResponsiveE-CommerceWebsite/
  index.html
  products.html
  product-detail.html
  cart.html
  style.css
  script.js
```

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript (ES6)
- Feather Icons (CDN)
- Google Fonts (Inter)

## How to Run Locally

Since this is a static project, no build step is required.

1. Open the project folder in VS Code.
2. Open `index.html` in your browser.

Recommended option:

- Use a local server extension like Live Server for best results with navigation and testing.

## Main Pages

- `index.html` - Home page with hero, featured products, categories, and newsletter
- `products.html` - Full catalog with filtering/sorting controls
- `product-detail.html` - Product detail view rendered from product ID in URL
- `cart.html` - Shopping cart and order summary

## Data and State Management

- Product catalog is stored in `script.js` as a static `PRODUCTS` array.
- Cart is stored in browser localStorage under key: `shopverse_cart`.
- Theme preference is stored in browser localStorage under key: `shopverse_theme`.

## Customization Guide

### Add or update products

Edit the `PRODUCTS` array in `script.js`.

Each product object includes fields like:

- `id`
- `name`
- `category`
- `price`
- `originalPrice`
- `rating`
- `reviews`
- `image` / `images`
- `description`
- `highlights`
- `brand`, `material`, `weight`, `warranty`

### Update styling

- Edit `style.css` for colors, spacing, layout, typography, and component styles.

### Update behavior

- Edit `script.js` for filtering logic, cart rules, coupon behavior, and page interactions.

## Notes

- This is a front-end demo project; there is no backend or real payment gateway.
- Product data and checkout are simulated for UI/UX demonstration.

## Future Improvements

- Integrate a backend API for products, users, and orders
- Add authentication and user accounts
- Add wishlist persistence
- Add pagination and server-side search
- Add unit/integration tests

## License

This project is for learning and portfolio use.
