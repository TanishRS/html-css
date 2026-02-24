# Portfolio

A personal profile/portfolio page with a video background, background music, a profile photo, and social media links.

## Files

| File | Description |
|------|-------------|
| `chota_project.html` | Main HTML page with the portfolio layout |
| `styles.css` | External stylesheet for animations, profile card, and social icons |
| `Tanish.jpg` | Profile photo |
| `3141207-uhd_3840_2160_25fps.mp4` | Looping background video |
| `Hans_Zimmer_-_Interstellar_Main_Theme_(mp3.pm).mp3` | Background audio |
| `Instagram.jpeg`, `github.png`, `Linkedin.png`, `X.jpeg` | Social media icons |

## HTML Concepts Used

- `<video>` with `autoplay`, `muted`, and `loop` attributes for a background video
- `<audio>` with `autoplay` and `loop` for background music
- `<img>` with `width` and `height` attributes for the profile photo
- `<a target="_blank">` for opening social links in a new tab
- Nested `<div>` containers for layout structure
- Inline image from an external URL (`cinema` meme image)

## CSS Concepts Used

- `position: fixed` with `inset: 0` for full-screen background layers
- `z-index` for controlling stacking of video, image, and content layers
- `opacity` for semi-transparent overlays
- `filter: hue-rotate()` applied to a background image
- `body::before` pseudo-element for a solid color underlay
- `@keyframes borderGlow` animation for a pulsing border effect
- `animation` property with `infinite` loop
- `transform: scale() rotate()` on `:hover` for profile image effect
- `border-radius: 50%` for circular social icon buttons
- `position: absolute` for social icons placed around the profile card
- `transition` for smooth hover effects
- `box-shadow` for a glowing ring effect
