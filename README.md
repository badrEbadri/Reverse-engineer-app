# Mon Ledger

A local-first personal finance journal built as a React progressive web app.

**Live app:** [https://badrebadri.github.io/Reverse-engineer-app/](https://badrebadri.github.io/Reverse-engineer-app/)  
**Repository:** [badrEbadri/Reverse-engineer-app](https://github.com/badrEbadri/Reverse-engineer-app)

## Features

- Track income and expenses by category.
- Review activity in the dashboard, transaction history, reports, and calendar.
- Manage categories and choose a language (French, English, or Arabic) and currency (MAD, EUR, USD, GBP, or CAD).
- Use the installable, offline-capable PWA.
- Export data as a complete backup, CSV, or JSON, and restore from a ZIP backup.

## Data and privacy

The app stores its data in IndexedDB in the visitor's browser. It has no account or cloud-sync feature, so data does not follow you to another browser or device. Export backups regularly; clearing browser data or losing the device can remove records that have not been backed up.

The GitHub Pages site and repository are public. Each visitor's app data is kept in that visitor's own browser storage.

## Repository contents

- `index.html` — app entry page.
- `assets/` — production JavaScript and CSS bundles.
- `manifest.webmanifest`, `sw.js`, and `workbox-*.js` — PWA installation and offline caching.
- `icon.svg`, `icon-192.png`, and `icon-512.png` — app icons.
- `.github/workflows/deploy-pages.yml` — GitHub Pages deployment workflow.

This repository currently contains the built static app, not the original React source project. It does not include `package.json` or an `npm run dev` command.

## Deployment

GitHub Actions publishes the static site to [GitHub Pages](https://badrebadri.github.io/Reverse-engineer-app/) whenever a commit is pushed to `master`. The workflow stages the app in `_site` and adjusts the built-in base path for the repository's Pages URL.

See [workflow runs](https://github.com/badrEbadri/Reverse-engineer-app/actions) for deployment status.
