---
layout: default
title: Experiment 7–8 — ES6 To-Do Application
permalink: /Lab/Exp_7-8/
---

# Experiment 7–8 — ES6 To-Do Application

**SAP ID:** 590014609

This experiment builds a browser-based to-do list using modern JavaScript (ES6+) and DOM event handling.

## Features

- Add tasks using the button or the Enter key.
- Mark tasks as complete by clicking the task.
- Delete tasks with the Delete button.
- Render the current task list dynamically in the browser.
- Create tasks with an ES6 `class` and update arrays with spread, `map()`, and `filter()`.

## Files

- `index.html` — page layout and styling.
- `app.js` — task model, event listeners, rendering, completion, and deletion logic.

## Run the experiment

Open `index.html` directly in a browser, or serve the folder locally:

```bash
python3 -m http.server 8000
```

Then, while the server is running, enter `http://localhost:8000` in your browser.

Tasks are stored in memory and will reset when the page is refreshed.
