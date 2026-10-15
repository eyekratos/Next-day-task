# NextDay Mobile PWA

A mobile-first daily planner you can add to your phone's home screen. It includes:
- Daily tasks with priority, category and time estimates
- Main win and notes for the day
- Roadmap steps for longer-term goals
- Daily reflection and progress summary
- Local browser storage and JSON backup/restore
- Basic offline caching after first load (when served over HTTPS)

## Run locally on Windows
This is a static website. For PWA install features, serve it over HTTPS or localhost (not by opening the HTML file directly).

With Python installed, open PowerShell in this folder and run:
```powershell
python -m http.server 8000
```
Open http://localhost:8000 in a browser. For phone testing on the same Wi-Fi, use a proper HTTPS deployment instead of localhost.

## Free hosting
1. Create a GitHub repository and upload `index.html`, `manifest.json`, `sw.js`, and `icon.svg`.
2. In the repository go to Settings → Pages.
3. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, then Save.
4. Wait for the published URL. Open it on your phone over HTTPS.

## Add to home screen
- Android Chrome: open the deployed HTTPS URL → browser menu (⋮) → Install app or Add to Home screen.
- iPhone Safari: open the HTTPS URL → Share → Add to Home Screen.

## Important data note
This starter stores tasks in the current browser's local storage. It does not sync automatically between devices, and clearing browser data can erase it. Use Export backup regularly. A shared login/database would be needed for secure cross-device sync. Browser notifications are permission-based and may not run reliably when the browser is closed; reliable scheduled push notifications require additional push/server setup.
