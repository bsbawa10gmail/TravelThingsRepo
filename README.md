Travel Checklist

A small, dependency-free web checklist for travel planning. Open `TravelThings.html` in a browser to run the app locally.

Files
- `TravelThings.html` — main app UI (open in browser).
- `inputItems.html` — helper page for adding items/input UI.
- `script.js` — app logic: loading/saving CSV, undo, checkbox handling.
- `styles.css` — visual styles.
- `travel_checklist.csv` — sample checklist / data import-export file.

Usage
- To use: open `TravelThings.html` in your browser (double-click or serve with a local static server).
- Import checklist state: use the "Load from CSV" control and select a CSV with columns `Section,Item,Checked`.
- Export checklist: use "Save Checklist as CSV" to download the current state.
- Undo: use the "Undo" control to revert the most recent change.

Editing the checklist
- Edit `travel_checklist.csv` directly to prepare a checklist for import, or add items via `inputItems.html` when provided in the UI.

Development
- No build tools required. For a simple local server (recommended for some browsers), run:

Running locally

- Double-click `TravelThings.html` to open the app in your browser (file://). The page contains an inlined script and will work without any build tools.

- If you prefer to serve files over HTTP (optional), you can run a simple static server:

Option A — Python (optional):
```bash
python -m http.server 8000

# then open http://localhost:8000/TravelThings.html
```

Notes
- The inlined script in `TravelThings.html` is the runnable copy for double-click usage. Development copy `src/main.js` has been removed; edit the inlined script directly or I can re-add a separate dev copy on request.
Questions or changes
- If you'd like a different README layout or additional instructions (installation, screenshots, or example CSV), tell me what you'd like included and I will update it.
