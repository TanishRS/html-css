# Offline Learning Notes

A single-page note-taking app that saves notes to `localStorage` so they persist without an internet connection. It also detects and displays the user's current online/offline status.

## Files

| File | Description |
|------|-------------|
| `index.html` | Single file with embedded CSS and JavaScript |

## HTML Concepts Used

- Google Font (`Nunito`) via `<link>`
- Embedded `<style>` block in `<head>`
- Embedded `<script>` block before `</body>`
- `<form id="notesForm">` for structured input submission
- `<input type="text">` for the topic name
- `<textarea>` for multi-line notes input
- `<button type="submit">` for saving notes
- `<button id="clearBtn">` for clearing saved notes
- `<div class="status">` for dynamic online/offline status display
- `<div class="card">` as the centered card container

## CSS Concepts Used

- CSS custom properties: `--pink`, `--pink-dark`, `--pink-soft`, `--white`, `--gray`, `--radius`
- `min-height: 100vh` + flexbox centering (`justify-content: center`, `align-items: center`) on `body`
- `background: linear-gradient(135deg, ...)` for the page background
- `box-shadow` for the card's depth effect
- `@keyframes fadeUp` entrance animation on the card
- `border-radius` on inputs, buttons, and the card
- `transition` on inputs for animated focus border and box shadow
- `box-shadow: 0 0 0 4px rgba(...)` on `input:focus` for a glow ring
- `linear-gradient` background on the save button
- `transform: translateY()` on button `:hover` for lift effect

## JavaScript Concepts Used

- `localStorage.setItem()` and `localStorage.getItem()` to save and load notes
- `localStorage.removeItem()` to clear saved notes
- `window.addEventListener("load", ...)` to restore saved values on page load
- `form.addEventListener("submit", ...)` with `e.preventDefault()` to handle saving
- `navigator.onLine` to check current connectivity status
- `window.addEventListener("online", ...)` and `window.addEventListener("offline", ...)` to listen for network changes
- `setTimeout()` to revert the status message after 3 seconds
- `confirm()` dialog for delete confirmation
