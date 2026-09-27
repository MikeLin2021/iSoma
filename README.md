# iSoma ECG & AI Platform — complete source

This package contains the canonical static files used to reproduce the iSoma ECG & AI Platform page.

## Run locally

1. Open a terminal in this folder.
2. Run `python3 -m http.server 8080 -d dist`.
3. Visit `http://localhost:8080` in a browser.

You may also open `dist/index.html` directly, although a local web server more closely matches normal hosting.

## Deploy

Upload the contents of `dist/` to the document root of any static hosting provider. The page has no build step and no server-side dependency.

## File inventory

- `dist/index.html` — complete semantic HTML page
- `dist/styles.css` — layout, responsive design, animation and visual styling
- `dist/script.js` — mobile navigation, journey tabs and reveal interactions
- `dist/assets/isoma-hero.png` — original hero artwork used by the page
- `.openai/hosting.json` — hosting metadata from the canonical project

## Media note

The canonical page contains no movie or video files and does not reference MP4, WebM, MOV or embedded video. Its visible motion is created by CSS and JavaScript. The included PNG is the only raster media asset required by the page.

## External dependency

The page requests the DM Sans and Manrope font families from Google Fonts. If an entirely offline copy is required, download appropriately licensed font files, place them under `dist/assets/fonts/`, and replace the Google Fonts links with local `@font-face` rules.
