# Beginner E-Commerce Page

A simple beginner-level e-commerce product listing page with an "Add to Cart" feature, a cart counter, and a total price calculator. All styles and JavaScript are embedded in the HTML file.

## Files

| File | Description |
|------|-------------|
| `index.html` | Single file with embedded CSS, HTML structure, and JavaScript |

## HTML Concepts Used

- `<header>` for the shop title
- `<div id="productList">` as the container for dynamically rendered product cards
- `<div id="cartBox">` with `<ul id="cartItems">` for the cart display
- `<span id="cartCount">` and `<span id="total">` for live data display
- `position: fixed` cart badge in the top-right corner
- Embedded `<style>` block inside `<head>`
- Embedded `<script>` block before `</body>`

## CSS Concepts Used

- `display: grid` with `grid-template-columns: repeat(auto-fit, minmax(220px, 1fr))` for the product grid
- `box-shadow` and `border-radius` for card styling
- `object-fit: cover` on product images for consistent sizing
- `position: fixed` for the floating cart counter badge
- `background-color` and `color` for button styling
- `button:hover` for a darkened hover state

## JavaScript Concepts Used

- Array of product objects (`id`, `name`, `price`, `img`)
- `forEach` + `document.createElement` to dynamically build product cards
- `innerHTML` template literal to inject card content
- `addToCart(id)` function using `Array.find()` to lookup a product
- `cart` array to store added items
- `updateCart()` function to re-render the cart list and recalculate total
- `innerText` for updating cart count and total price in the DOM
