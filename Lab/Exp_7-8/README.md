---
layout: default
title: Experiment 7–8 — ES6 To-Do Application
permalink: /Lab/Exp_7-8/
---

# Experiment 7–8 — ES6 To-Do Application

**SAP ID:** 590014609

**Course:** Backend Development

---

## 🎯 Aim & Objectives

### Aim
To build an interactive browser-based to-do application using ES6 classes, DOM manipulation, event listeners, and immutable-style array updates.

### Key Objectives
1. Create a reusable task model with an ES6 class.
2. Capture user input and keyboard events.
3. Render dynamic data in the DOM.
4. Toggle task completion and delete tasks.
5. Use spread syntax, `map()`, and `filter()` to update state.

---

## 📚 Theoretical Background

The Document Object Model (DOM) represents an HTML page as objects that JavaScript can read and modify. Event listeners respond to user actions, while array methods help maintain the application's in-memory task state without directly mutating the existing collection.

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

---

## 💻 Practice Tasks

1. Add a task from a button click.
2. Add a task when the user presses Enter.
3. Toggle a task between complete and incomplete.
4. Delete a task from the list.
5. Re-render the task list after every state change.

---

## 📌 Conclusion

This experiment demonstrates how modern JavaScript and DOM event handling can be combined to create an interactive client-side application.
