# Photography Portfolio

A dark, editorial-style photography portfolio with a fixed nav, full-screen hero, horizontally scrollable gallery, about section, quote block, contact form, and footer. All styles are embedded in the HTML file.

## Files

| File | Description |
|------|-------------|
| `index.html` | Single file with embedded CSS and full page layout |

## HTML Concepts Used

- Google Fonts (`Playfair Display`, `Inter`) via `<link>`
- Embedded `<style>` block inside `<head>`
- Semantic elements: `<nav>`, `<section>`, `<footer>`, `<ul>`, `<li>`, `<a>`
- `<button class="btn">` for CTA and form submit
- `<input type="text">`, `<input type="email">`, `<textarea>` for contact form
- Multiple `<section>` elements named `.hero`, `.gallery-section`, `.about`, `.quote`, `.contact`
- Gallery built with individual `.card` divs each containing an `<img>` and an overlay `<div>`
- `<img>` loaded from external Pinterest/Unsplash/Picsum URLs

## CSS Concepts Used

- CSS Reset (`* { margin:0; padding:0; box-sizing:border-box; }`)
- `position: fixed` + `z-index` for sticky navbar
- `background: linear-gradient(to bottom, rgba(...), transparent)` for navbar fade overlay
- `height: 100vh` + `background: url(...) center/cover` for the hero
- `::after` pseudo-element with `background: rgba(0,0,0,...)` hero dark overlay
- `display: flex` + `overflow-x: auto` for the horizontal scrolling gallery
- `::-webkit-scrollbar { display: none; }` to hide the scrollbar
- `transform: scale(1.1)` on image `:hover` with `transition` for a zoom effect
- `position: absolute; inset: 0` on `.card-overlay` for text over image gradient
- `display: grid` with `grid-template-columns: 1fr 1fr` for the about section
- `@media (max-width: 900px)` for single-column layout on smaller screens
- Dark color palette: `#0e0e0e` background, `#f5f5f5` text
- `font-family: 'Playfair Display'` for headings, `'Inter'` for body text
