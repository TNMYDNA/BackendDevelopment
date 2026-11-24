# Lecture 7 — Browser Storage and JSON

This lecture explores browser storage APIs and JSON serialization. The examples use `localStorage`, `sessionStorage`, `JSON.stringify()`, and `JSON.parse()` to save and retrieve data in the browser.

## Topics covered

- Saving, reading, removing, and clearing `localStorage` values.
- Using temporary `sessionStorage` data.
- Converting JavaScript objects to JSON strings and back again.
- Storing simple objects, nested objects, and arrays of objects.
- Creating reusable `save()` and `load()` storage helpers.
- Inspecting stored values with browser DevTools.
- Building a Notes/Todo app backed by `localStorage`.

## Run the examples

Open any HTML file directly in a browser, or serve this folder with a local web server. For example:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) and select an exercise.

Open the browser developer tools to view the console output and inspect stored values under the browser's Storage or Application panel.

## Final task

Open `Final-Task-Notes-App.html` to use the Notes/Todo app. It supports:

- Adding notes
- Editing notes
- Marking notes complete
- Deleting notes
- Persisting notes in `localStorage`

Stored notes remain available after refreshing the page until the site's storage is cleared.
