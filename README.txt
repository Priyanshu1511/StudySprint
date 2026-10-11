# StudySprint — Exam Tracker

A no-login, static study-tracking website for Priyanshu and Sona.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in Chrome, Edge, Firefox, or Safari.
3. Use the sidebar to track lectures, mock tests, and Geography topics.

## Features
- Visual dashboard and subject progress bars
- 150 pre-created lecture slots (50 each for Reasoning, Maths, English)
- Completion toggles and three revision date fields
- Mock test tracking for Testbook and Oliveboard
- Sona's Geography branches, PDF links, mock accuracy, and revision status
- Personal Call Journal: manually log incoming/outgoing/missed/video calls, duration, purpose, notes, follow-up status, and optional permitted recording links
- Search/filter, edit/delete, print, JSON export and import
- Personal call-session logs (metadata and follow-ups; no automatic phone-call recording)
- Meetup planner with Google Meet/Calendar links
- Diary entries, messages to one another, voice-note recording/upload/playback (browser-local)
- Daily wellness routine: optional aloe vera juice, yoga, meditation, Surya water offering, temple, diet, water, activity, revision, outside food, wake/sleep times
- No login and no external libraries required

## Data and privacy
This is a static, browser-based app. Text records are stored in the current browser's local storage and audio blobs in browser IndexedDB. They are not uploaded to a server.
- Use **Export backup** regularly.
- To move data to another browser/device, export a JSON backup and import it there.
- This build does not automatically synchronize data between Priyanshu and Sona or between devices.
- Call Journal is a manual record-keeping feature. It does not record phone-call audio, access call history, or monitor calls automatically. Only save recording links when you have the necessary consent and legal permission.
- If you host the website publicly, the site itself can be opened without login, but each visitor's data remains in that visitor's browser. Anyone with the URL can use the app and save their own local data.

## Google Drive PDFs
Upload the PDF to Google Drive, set sharing access for the intended viewer, copy its link, and paste it into the PDF link field. Anyone opening the link must have the required Drive permission.

## Publish without login using GitHub Pages
1. Create a GitHub repository (e.g. `exam-tracker`).
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
5. Wait for the Pages URL shown in Settings → Pages. The website itself does not require login for visitors.

Note: GitHub requires your own account to create/manage the repository, but visitors do not need a GitHub account to open a public Pages site.

## New personal sections
- **Call records:** manually log person, time, duration, call type, notes, and follow-up. This does not access or record phone calls automatically.
- **Meetups:** save meeting date/time, attendees, agenda, location, and a Google Meet URL. Actual Google Calendar event creation and Meet link generation require Google integration; this no-login build only stores details and opens the official services.
- **Diary & messages:** add entries and leave messages for Priyanshu/Sona.
- **Daily voice notes:** use microphone recording (Chrome/Edge may require HTTPS or localhost), upload audio, playback, download, and delete. Audio is local to the browser and is not included in the JSON backup.
- **Daily wellness:** track wake/sleep time, optional aloe vera juice, yoga, meditation, Surya Bhagwan water offering, temple/prayer, balanced meals, hydration, revision minutes, activity, outside food, mood, and notes.
