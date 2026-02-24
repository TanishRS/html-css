# Mini Project — Pong Game

A browser-based two-player Pong game built with plain HTML, CSS, and JavaScript.

## Files

| File | Description |
|------|-------------|
| `ping_pong2.html` | Main page with the landing layout and the embedded game logic |
| `style.css` | External stylesheet for the landing page and game UI |

## HTML Concepts Used

- Semantic elements: `<nav>`, `<footer>`, `<aside>`, `<section>`
- `<canvas>` element for rendering the game
- Inline `<script>` block for game logic
- External Google Font (`Press Start 2P`) via `<link>`
- `<button>` with `onclick` attribute to trigger the game

## CSS Concepts Used

- CSS Reset (`* { margin: 0; padding: 0; box-sizing: border-box; }`)
- `background-image` with an inline SVG data URI for a tiled background
- Flexbox for layout (`.content`, `.nav`, `.game-buttons`)
- `linear-gradient` for container background
- `position: fixed` for the full-screen game canvas overlay
- `display: none` / `display: flex` for show/hide toggle
- Responsive centering with `width` + `margin: 0 auto`

## JavaScript Concepts Used

- `<canvas>` 2D context (`getContext("2d")`)
- `requestAnimationFrame` game loop
- Keyboard event listeners (`keydown` / `keyup`) for paddle controls
- Object literals for game state (paddles and ball)
- Collision detection between ball and paddles
- Ball reset on scoring (ball goes off screen)
