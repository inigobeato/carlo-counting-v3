CARLO COUNTING — LIFETIME-FOCUSED BUILD

FILES
- index.html: complete application
- manifest.webmanifest: installable app metadata and icons
- sw.js: app-shell caching for offline opening after first successful visit
- icons/: app icons

DEPLOY
Upload the CONTENTS of this folder to the root of your GitHub repository. Keep the icons folder. Netlify should publish from the repository root.

IMPORTANT DATA SAFETY
This edition stores business records in the browser's local storage on the current device/browser profile. It does not provide automatic cloud sync or multi-device conflict handling. Export a JSON backup after each business day and store copies in at least two separate places. Before restoring, the app downloads a safety copy of current data. Do not clear browser storage or uninstall/reset the browser without first exporting a backup.

OFFLINE
The service worker caches the app shell for repeat visits after the first successful online load. Offline access does not synchronize records.

TEST AFTER DEPLOYMENT
1. Add a test reviewer and record a test sale.
2. Edit and delete the test sale; confirm totals and stock.
3. Add an expense and verify net income.
4. Export a JSON backup, then test restore using a copy.
5. Install the app from Chrome.

SIDEBAR LOGO FIX:
The sidebar now displays your uploaded CARLO COUNTING logo. Keep icons/sidebar-logo.png in the icons folder when uploading. The service worker cache was updated to v4.


SIDEBAR LOGO FIX (v5)
- Sidebar logo is embedded directly in index.html to prevent missing/case-sensitive path issues on hosting.
- Logo area has a fixed responsive display height and centered contain fit.
- Service-worker cache was versioned to v5 so browsers replace the previous app.
After uploading: redeploy the complete folder, then fully close and reopen the app. If an installed PWA still shows the old version, open the site in Chrome and reload.
