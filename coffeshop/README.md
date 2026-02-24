# Coffee Shop Website

A multi-section coffee shop website with a hero, about, menu, contact form, and footer, with external fonts and a separate CSS file.

## Files

| File | Description |
|------|-------------|
| `index.html` | Main HTML with all page sections |
| `style.css` | External stylesheet for the full page |

## HTML Concepts Used

- Semantic elements: `<nav>`, `<section>`, `<footer>`, `<form>`
- Google Fonts (`Cormorant Garamond`, `Montserrat`) via `<link rel="preconnect">`
- `<form>` with `<input type="text">`, `<input type="email">`, `<textarea>`, and `<button type="submit">`
- `href="#id"` anchor links in the navigation for smooth in-page scrolling
- `<img>` with `alt` text and local image references
- Organised content into named sections: `#home`, `#about`, `#menu`, `#contact`
- Emoji characters used as feature icons (`☕`, `🎨`, `🌿`, `📍`, `⏰`, `📞`)

## CSS Concepts Used

- External stylesheet linked via `<link rel="stylesheet">`
- Flexbox for navbar layout and about/contact two-column layouts
- `position: relative` hero section with layered `<div>` overlays
- `scroll-indicator` decorative element using flex and a thin line div
- CSS class conventions: `section-title`, `title-underline`, `menu-grid`, `menu-category`, `menu-item`
- `display: grid` for the three-column menu grid
- `box-shadow` and `border-radius` for card styling
- Transition effects on buttons (`:hover` state)
- `max-width` + `margin: auto` for centered content containers
- `padding` and `margin` for spacing between sections
