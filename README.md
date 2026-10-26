# Drive: Live Speed & Trip

An installable web app (PWA) that shows live speed, distance, heading, altitude and trip stats using your phone's GPS. No build step, no dependencies.

## Files
- `index.html`: the whole app
- `manifest.webmanifest`: install details (name, icons, colours)
- `sw.js`: service worker for offline use
- `icons/`: app icons (Android, iPhone, maskable)
- `vercel.json`: hosting headers

## Deploy
1. Create a GitHub repo and upload everything in this folder to its root (so `index.html` sits at the top level).
2. In Vercel: **Add New > Project**, import the repo, leave Framework Preset as **Other**, and click **Deploy**. No build command is needed.
3. Open the Vercel link on your phone, allow location, then **Install** (Android/Chrome) or **Share > Add to Home Screen** (iPhone).

## Updating
Edit a file, then change `VERSION` in `sw.js` (for example `drive-v2`) so installed copies pick up the change.

## Notes
- Location only works on HTTPS pages. Vercel provides HTTPS automatically.
- Use **Try demo** in the app to preview without GPS.
