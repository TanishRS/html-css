# Design Tool Landing Page

A Figma-inspired landing page with a hero section, canvas-drawn graphic, CTA buttons, and a trusted-brands strip.

## Files

| File | Description |
|------|-------------|
| `index.html` | Main HTML page with layout structure and inline canvas script |
| `style.css` | External stylesheet for navigation, hero, buttons, and responsive styles |

## HTML Concepts Used

- Semantic `<nav>` and `<section>` elements
- `<canvas>` element with `id="heroCanvas"` for the right-side graphic
- Inline `<script>` block for canvas drawing
- `<a>` tags inside nav styled as text links
- `<div>` containers for button groups and layout sections

## CSS Concepts Used

- CSS Reset with `box-sizing: border-box`
- `background: linear-gradient(135deg, ...)` on `body` for a soft gradient background
- Flexbox on `nav` (`justify-content: space-between`) and `.hero` (`align-items: center`)
- `-webkit-background-clip: text` + `-webkit-text-fill-color: transparent` for gradient text on the `<h1>`
- `backdrop-filter: blur()` for a frosted-glass effect on the canvas card
- `box-shadow` with rgba for soft depth
- `transition` + `transform: translateY()` on button `:hover`
- `border-radius` on the canvas container and CTA button
- `@media (max-width: 900px)` to stack hero columns vertically

## JavaScript (Canvas API) Concepts Used

- `getContext("2d")` to access the 2D drawing context
- Drawing a grid with `beginPath()`, `moveTo()`, `lineTo()`, and `stroke()`
- `createLinearGradient()` to create gradient fills
- `addColorStop()` to define gradient color points
- `fillRect()` to draw colored rectangles
- `fillText()` to draw labels inside the rectangles
