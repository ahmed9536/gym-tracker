GYM TRACKER — VERSION 1

Files:
- index.html: the app
- manifest.webmanifest: Android install metadata
- sw.js: offline app-shell cache

Quick test:
Open index.html in Chrome on Android or a desktop browser. Data is stored in that browser's local storage.

Important Android install note:
For the full installable PWA experience (Add to Home Screen + service-worker offline cache), serve these files from an HTTPS website. A service worker cannot be installed from a file:// URL. You can publish this folder using GitHub Pages or another static HTTPS host. Open the HTTPS link in Chrome, choose the browser menu, then "Install app" or "Add to Home screen". After the first successful load, the app shell is cached and can open offline.

Data:
- Workout data stays on this device/browser.
- Export a JSON backup regularly.
- Import replaces the current local data.
- Notes are required for every set before finishing a workout.
- Timer duration is calculated from timestamps, so it remains accurate if the screen sleeps or the app is backgrounded.
