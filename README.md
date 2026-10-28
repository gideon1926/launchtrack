# LaunchTrack

A responsive job application tracker built with HTML, CSS, and vanilla JavaScript. Created with AI assistance as a learning project for Gideon's web development portfolio.

## Features
- Add, edit, and delete applications with company, role, location, date, status, and notes.
- Filter by status and search by company, role, or location.
- Summary counts for applications, interviews, and offers.
- Local browser persistence and CSV export, including spreadsheet formula escaping.
- Responsive layout, labeled forms, keyboard focus states, and native modal dialog.

## Run locally
Open `dist/index.html` in a modern browser, or serve the folder:

```sh
python -m http.server 8000 --directory dist
```

Visit http://localhost:8000. No dependencies or build step required.

## Structure
- `dist/index.html`: semantic page and form.
- `dist/style.css`: responsive visual design.
- `dist/app.js`: state, rendering, CRUD, persistence, and export.

## Data and privacy
Application data stays in localStorage in the current browser profile. There is no backend, login, cross-device sync, or recovery service. Clearing browser data removes saved records. CSV export is a backup download; CSV import is not implemented. Notes may contain personal information, so use a trusted device.

## Manual checks
1. Add an application, reload, and confirm persistence.
2. Edit its status and verify summary counts and filters.
3. Search by company and role; verify the empty state.
4. Export CSV and verify quoted commas, line breaks, and formula-like text.
5. Cancel deletion and then confirm deletion.
6. Use the form with the keyboard and check the layout at mobile width.

## Learning roadmap
Understand and modify the DOM rendering and state updates before presenting this as interview work. Useful next steps include automated browser tests, CSV import, React migration, and a backend with authentication.
