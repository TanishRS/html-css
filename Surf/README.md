# Surf Academy Landing Page

A multi-section landing page for a fictional surf academy, featuring a hero, about, courses, gallery, and footer.

## Files

| File | Description |
|------|-------------|
| `surf.html` | Main HTML page with all page sections |
| `styles.css` | External stylesheet for layout, typography, and responsive design |

## HTML Concepts Used

- Semantic elements: `<nav>`, `<section>`, `<footer>`
- `<h1>`, `<h2>`, `<h3>` heading hierarchy
- Unordered list `<ul>` / `<li>` for navigation links
- `<img>` with `src` from Unsplash URLs and `alt` text
- `<button>` inside the hero section
- Multiple `<section>` elements for page structure

## CSS Concepts Used

- CSS Reset (`* { margin: 0; padding: 0; box-sizing: border-box; }`)
- `linear-gradient` overlay on a background image for the hero section
- `background-image`, `background-size: cover`, `background-position: center`
- `height: 100vh` for a full-screen hero
- Flexbox for navigation (`justify-content: space-between`, `align-items: center`)
- `display: inline-block` for course cards
- `border-radius`, `overflow: hidden`, `box-shadow` for card styling
- `transition` + `transform: translateY()` on `:hover` for card lift effect
- `object-fit: cover` on images inside cards and gallery
- `@media` query for basic responsive layout
