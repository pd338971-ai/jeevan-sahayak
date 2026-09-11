# Jeevan Sahayak — Real App / PWA Edition

This is an installable Progressive Web App (PWA) prototype.

## Added features
- Installable app experience on supported browsers
- Offline cache/service worker
- Local account + PIN gate
- Dark/light mode
- Tasks with edit/delete/done
- Date/time reminders
- Browser notification permission and in-app reminder fallback
- Medicine time reminders
- Expenses + monthly budget
- Expense chart
- Water tracker
- Daily habits
- Notes
- Trusted contacts + call button
- Search
- CSV export (opens in Excel)
- Print report -> Save as PDF
- Full JSON backup/restore
- Responsive mobile/desktop UI

## Run locally
Because service workers generally require HTTPS or localhost, use a local server:
- Python: `python -m http.server 8000`
- Then open `http://localhost:8000`
Or deploy the folder to an HTTPS static host.

## Install on phone
Open the HTTPS/localhost app in a supported browser and choose Install/Add to Home Screen.

## Production note
This edition is a real installable PWA, but its account is local-only. For a true multi-device production app, add a secure backend (HTTPS, hashed passwords, sessions/JWT, database, server-side validation, rate limiting, backups and push-notification infrastructure). Do not use this local PIN system for sensitive data.

## Notifications
While the app is open, the reminder checker can show browser notifications when permission is granted. Reliable background reminders while the app is completely closed require a server/push or platform-specific scheduling system.

## Version 3.0 additions
- Daily Goals with progress
- Calendar/day planner
- Achievement badges
- Habit/task streak indicator
- Expanded dashboard
- Goals included in export
