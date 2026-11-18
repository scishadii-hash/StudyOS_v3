# StudyOS v3 — Modular PWA prototype

## Included
- IndexedDB database (`courses`, `lectures`, `meta` stores)
- Course CRUD: create, read, update, delete
- Lecture CRUD: create, read, update, delete
- Weekly planner generated from lecture records
- JSON backup export and restore
- Light/Dark theme and English/Arabic interface
- Service worker app-shell caching for offline use after first successful load
- Responsive desktop/mobile navigation

## Run locally
For IndexedDB and service-worker behavior, serve this folder from localhost or HTTPS. Opening `index.html` directly with `file://` will not enable service-worker offline caching and may restrict browser storage.

## Deploy
Upload the contents of this folder to the root of a GitHub Pages repository (keep `index.html`, `styles.css`, `app.js`, `manifest.json`, and `sw.js` together). Open the HTTPS Pages URL once while online; then reload once to let the service worker cache the app shell.

## Data and backup
Student data is stored locally in IndexedDB. Export JSON regularly and keep a copy outside the app. Clearing browser/site data or uninstalling a browser profile may remove local data. Restore replaces the current course and lecture records.

## Current scope
This is a functional prototype, not a production release. Accounts, cloud sync, notifications, grades, and focus timer are intentionally not implemented in this build.
