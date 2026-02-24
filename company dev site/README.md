# Robotics Studio Company Site

A dark-themed, full single-page company website for a robotics studio, including a hero, stats bar, services, projects portfolio, process steps, contact form, and footer. All styles are embedded in the HTML file.

## Files

| File | Description |
|------|-------------|
| `index.html` | Single file with embedded CSS and full HTML layout |

## HTML Concepts Used

- Semantic elements: `<nav>`, `<section>`, `<footer>`, `<form>`
- Google Fonts (`Orbitron`, `DM Sans`) via `<link>`
- Embedded `<style>` block with all CSS inside `<head>`
- `<ul>` / `<li>` / `<a>` for the navigation menu
- `href="#id"` anchor links for in-page navigation
- `<input type="text">`, `<input type="email">`, `<textarea>` for the contact form
- `<button type="submit">` for form submission
- Background image set via inline CSS `background-image: url(...)`

## CSS Concepts Used

- CSS custom properties in `:root`: `--cyan`, `--cyan-dim`, `--dark`, `--text`, `--white`
- `position: fixed` with `backdrop-filter: blur()` for the sticky frosted glass navbar
- `::before` and `::after` pseudo-elements for hero overlays and animated grid
- `@keyframes gridMove` for an infinitely scrolling background grid animation
- `@keyframes fadeUp` for the hero content entrance animation
- `display: grid` with `repeat(auto-fit, minmax(..., 1fr))` for services, projects, and steps
- `transition` + `transform: translateY()` on card `:hover`
- `box-shadow` with glow effects on hover using `rgba` cyan color
- `border-radius` on cards and buttons
- `scroll-behavior: smooth` on `body`
- `overflow-x: hidden` to prevent horizontal scroll
- `@media (max-width: 600px)` for mobile responsive adjustments (hidden nav links, stacked form grid)
- `letter-spacing`, `text-transform: uppercase` for the futuristic typography style
