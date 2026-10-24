# Kitchen Tracker

Table orders, kitchen queue, receipts and sales for a food stall. Works on a phone, installs like an app, and keeps working without signal.

No build step and no dependencies: it is plain HTML, CSS and JavaScript.

## Run it on your computer
Service workers need `http://`, not a double-clicked file, so start a tiny server in this folder:

    python -m http.server 5500

Then open http://localhost:5500 (or use the Live Server extension in VS Code).

## Publish it with GitHub Pages
1. Create a new repository on GitHub (for example `kitchen-tracker`).
2. Upload everything in this folder, keeping the `icons` folder.
3. Go to **Settings → Pages**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, then **Save**.
4. After a minute your app is at `https://YOUR-USERNAME.github.io/kitchen-tracker/`.

## Install it on a phone
Open the GitHub Pages link in Chrome, tap the ⋮ menu, then **Install app** (or **Add to Home screen**). Share the same link with friends so they can install it too.

## Good to know
- Orders, prices and receipts are saved in each phone's own browser storage. Nothing is sent anywhere, and each person sees only their own data.
- Clearing the browser's site data erases that phone's saved orders and receipts.
- When you change the app, edit `CACHE` in `sw.js` (for example `kitchen-tracker-v2`) before uploading, so phones fetch the new version.
