# 90-Day Path — Bruce Lee Protocol PWA

A binary habit tracker for the 90-Day Bruce Lee Protocol, deployable as a Progressive Web App via GitHub Pages.

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `90day-path`)
2. Upload all files in this folder to the repo root:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/icon-192.png`
   - `icons/icon-512.png`
   - `.nojekyll`
3. Go to **Settings → Pages → Source** → select `main` branch, `/ (root)`
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`

## PWA Features

- **Offline support** — full cache-first strategy via Service Worker
- **Installable** — Add to Home Screen banner on Android/iOS/Desktop
- **Today shortcut** — "Today" button scrolls to the current day row, highlighted in gold
- **Offline badge** — visible indicator when the network is unavailable
- **Auto-update** — SW checks for updates every 30 minutes in the background
- **Safe-area support** — notch/island-aware padding on iOS

## Data Storage

All data is stored in `localStorage` — no server, no account needed. Data stays on your device.

## File Structure

```
/
├── index.html       ← App shell + tracker UI
├── manifest.json    ← PWA manifest
├── sw.js            ← Service Worker (cache-first)
├── .nojekyll        ← Prevents Jekyll processing on GitHub Pages
└── icons/
    ├── icon-192.png
    └── icon-512.png
```
