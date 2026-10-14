# PMBridge

Project cards with task cards, schedule cards, quick-add dates and a month calendar.
Same look as Canvas and MYCAL. One static page, no build step.

## Files
- `index.html` – the whole app
- `manifest.webmanifest`, `icons/` – home-screen app name and icons
- `sw.js` – lets the app open offline
- `vercel.json` – makes sure phones always get the newest version

## Put it online
1. Create a new GitHub repo (for example `pmbridge`) and upload everything in this folder to the top level.
2. In Vercel: **Add New → Project → Import** that repo. Framework preset: **Other**. No build command, no output folder. Deploy.
3. Open the Vercel link on each device.

## Add to the home screen
- **iPhone / iPad:** open the link in Safari → Share → **Add to Home Screen**.
- **Computer (Chrome or Edge):** click the install icon in the address bar.

## Your data
Data is saved on each device in the browser (it survives closing the app and restarting the device).
Each device keeps its own copy, and on iPhone/iPad the home-screen app keeps a copy separate from Safari.
Use the **⋯** button → *Back up my data* to download a backup file, and *Restore from a backup file* to load it on another device.

## Updating
After changing any file, raise `VERSION` in `sw.js` (for example `pmbridge-v2`) so installed copies refresh.
