# NextDay Mobile V2

Mobile-first PWA productivity planner. Features:
- Daily task list with priority, categories, time estimates
- Select a date to plan future days
- Main win and note for each date
- Roadmap goals and milestones
- XP points, level labels, and completed-day streak
- 15/25/45-minute focus timer
- Last 7 days progress view and daily reflection
- Reminder preference and browser notification permission
- Export/import JSON backup
- Basic offline cache

## Update existing GitHub Pages site
1. Extract this ZIP.
2. Open your GitHub repository `Next-day-task`.
3. Add file → Upload files.
4. Upload/replace `index.html`, `manifest.json`, `sw.js`, and `icon.svg` at repository root.
5. Commit changes to the `main` branch.
6. Wait for GitHub Pages to deploy. Refresh the website on phone; if old version remains, close/reopen it or clear that site's cache.

## Reminder limitations
The reminder setting checks while the page is open. Browser notifications may work only after permission is granted and the app is active. Reliable notifications when fully closed require push infrastructure or a native Android app.

## Data note
Data is stored locally in this browser using localStorage. It does not sync between devices. Export a backup before clearing browser data.
