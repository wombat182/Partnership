# Wombat — site

Three pages plus a 404. HTML, CSS, and a small JavaScript animation on the home page.

## Files

- `index.html` — home (animated silhouette, separate wordmark text, three nav links)
- `about.html` — company description + contact
- `wombats.html` — wombat photo placeholders
- `404.html` — graceful page for mistyped URLs
- `style.css` — all styling
- `wombat-logo.png` — silhouette only, transparent background

## Logo structure (important)

The PNG file is **just the wombat silhouette** — no wordmark, no background. This way:

- Only the animal moves during the animation (the "wombat" wordmark is real HTML text below)
- The transparent background means the logo adopts whatever page color it's on — no color mismatch ever

If you ever swap the logo file, keep the same name (`wombat-logo.png`) and it should be a transparent silhouette with no text.

## Animation (home page)

Three behaviors composed onto a single transform, JS-driven:

1. **Breathe** — gentle continuous scale pulse
2. **Sprint** — every 22 seconds, the wombat runs to the right with a small bounce, pauses briefly, then walks slowly back with a subtle bob
3. **Look around** — every 35 seconds, a brief leftward shift

Hover pauses the motion and perks up the wombat. Honors `prefers-reduced-motion`.

## Editing

- **Email**: search `teigstad@icloud.com` in `about.html`
- **About paragraph**: edit `<p>` tags inside `.content` div in `about.html`
- **Org.nr**: search `925&nbsp;629&nbsp;634` across HTML files
- **Partners link**: search for `docs.google.com` in `index.html` to update the URL
- **Add a photo**: in `wombats.html` replace `<div class="placeholder">photo 1</div>` with `<img src="myphoto.jpg" alt="">`

## Colors

- Cream background: `#F5EFE0`
- Brown: `#3E2C1C`
- Soft brown (italic, captions): `#6b5742`

## Typography

EB Garamond (Google Fonts), Garamond/Times fallback. The wordmark on the home page now uses real EB Garamond instead of the rasterized text from the original logo file.
