# Vintage Books Store

A single-page vintage bookstore with a hero section, a dynamically rendered book grid, a modal for book details, and a sliding cart panel. All styles are written inline in the HTML file.

## Files

| File | Description |
|------|-------------|
| `index.html` | Single file containing HTML structure, embedded CSS, and JavaScript |

## HTML Concepts Used

- Semantic elements: `<nav>`, `<section>`, `<footer>`
- CSS custom properties (variables) defined in `:root`
- Google Fonts (`Playfair Display`, `Cormorant Garamond`) via `<link>`
- Embedded `<style>` block inside `<head>`
- `<button>` for cart toggle and "Add to Cart" action
- `<span>` with `id` attributes for dynamic JavaScript updates
- Modal overlay `<div>` built with `position: fixed; inset: 0`

## CSS Concepts Used

- CSS custom properties: `--burgundy`, `--gold`, `--parchment`, `--dark`
- `display: grid` with `grid-template-columns: repeat(auto-fit, minmax(250px, 1fr))` for the book grid
- `display: grid` with two equal columns for the modal layout
- `position: fixed` for the modal, cart drawer, and "close" button
- `transition` + `transform: translateY() scale()` on card `:hover`
- `box-shadow` for depth on cards and modal
- `overflow: auto` on the cart panel for scrollable cart items
- Slide-in cart with `right: -400px` / `right: 0` toggled via `.open` class
- `@media` query for stacking modal columns on small screens

## JavaScript Concepts Used

- Array of book objects with `title`, `price`, `img`, and `desc` properties
- `forEach` + `document.createElement` to dynamically build and append card elements
- `onclick` handler on each card to open a modal with book details
- `cart` array to track added items
- DOM manipulation to update cart item list and total
- `display: flex` toggled to show/hide the modal
- `classList.toggle("open")` for the sliding cart panel
