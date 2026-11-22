# RISO V2.0 — The Calm Strategist

## Files
- `index.html` — the app itself (HTML, CSS and JavaScript are together in this beginner-friendly version).
- `manifest.webmanifest` — tells supported browsers how the app should appear when installed.
- `sw.js` — service worker for offline caching.
- `icon.svg` — app icon.
- `README.md` — these instructions.

## Run it
1. Extract the ZIP.
2. Open `index.html` in a browser to preview the app. Some PWA/offline features require hosting over HTTPS or localhost.
3. For a live GitHub Pages website, upload the four app files (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`) to the same repository folder and commit the changes.
4. Open the GitHub Pages site in Chrome. Use the browser's Install app / Add to Home Screen option if available.

## Existing RISO V1.2 progress
On first launch, V2.0 checks the existing browser storage key `riso12` and migrates supported values (XP, streak, name, aim, targets, custom missions, and calendar notes). It leaves the original `riso12` key in place as a safety copy. Existing V1.2 completed missions for the current day are carried over as legacy completions.

Important: browser storage is local to the browser profile and device. A website update normally keeps it if you use the same domain and browser profile. If you clear browser data, switch browsers/devices, or use a different domain, the old data may not be available. Export a JSON backup before replacing a live app whenever possible.

## Current scope
- No AI, chatbot, external AI API, wearable connection, or health-data integration.
- The scheduler is deterministic rule-based logic.
- Fitness content is general beginner guidance, not medical advice.
- The current release is the personal development app update only. Wearable integration and health tracking are future separate development phases and are not implemented here.

## Data
The app stores its state in browser LocalStorage under `riso20`. The original `riso12` key is retained after migration. Use More → Backup & restore to export or restore a V2 JSON backup.
