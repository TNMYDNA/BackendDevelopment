---
layout: default
title: Experiment 10: jQuery DOM Manipulation and AJAX
---

# Experiment 10: jQuery DOM Manipulation and AJAX

**Course:** Backend Development  
**(SAP:- 590014609)**

---

## 🎯 Aim & Objectives

### Aim
To understand jQuery syntax and use it for DOM selection, content and style manipulation, visual effects, and asynchronous data exchange through AJAX requests.

### Key Objectives
1. **jQuery Setup**: Include jQuery in a web page and execute code after the DOM has loaded.
2. **Selectors and Events**: Select elements with IDs, attach click handlers, and respond to user actions.
3. **DOM Manipulation**: Modify classes, styles, text, HTML content, and child elements using jQuery methods.
4. **Visual Effects**: Apply fade, slide, show, and hide animations to page elements.
5. **AJAX Requests**: Retrieve JSON data asynchronously using both `$.ajax()` and `$.getJSON()`.
6. **Error Handling**: Handle failed requests and provide loading, success, and error feedback to the user.

---

## 📚 Theoretical Background

### jQuery
jQuery is a JavaScript library that simplifies DOM traversal, event handling, animation, and asynchronous HTTP requests through a concise API.

### Selectors and DOM Methods
jQuery selectors such as `$("#id")` and `$(".class")` locate elements. Methods including `.text()`, `.html()`, `.append()`, `.css()`, `.addClass()`, and `.removeClass()` update the page dynamically.

### Effects and Animations
Methods such as `.fadeToggle()`, `.slideToggle()`, and `.show()` create visual transitions without manually changing CSS display or opacity properties.

### jQuery AJAX
- **`$.ajax()`** provides detailed control over the request URL, method, expected data type, success callback, and error callback.
- **`$.getJSON()`** is a shorthand method for retrieving JSON data and handling the result with `.done()` and `.fail()`.

### Asynchronous Programming
AJAX requests run asynchronously, allowing the page to remain usable while data is being retrieved. Once the response arrives, the table and status message are updated without a full page reload.

---

## 💻 Practice Tasks

### Program 1: DOM Manipulation and Visual Effects

Use jQuery to:

- Toggle a highlight class on an interactive box.
- Fade and slide the box in or out.
- Change its text content dynamically.
- Append an element to the box.
- Reset the box to its initial state.

### Program 2: Asynchronous JSON Retrieval

Use `$.ajax()` and `$.getJSON()` to load `students.json`, render student records in a table, and display the current request status.

### Program 3: Error Handling

Request a missing JSON file to demonstrate how jQuery catches an HTTP error and displays an appropriate message to the user.

---

## 📁 Files

- `index.html` – Page layout, controls, student table, and jQuery CDN reference.
- `style.css` – Styling for the interactive cards, buttons, table, and feedback states.
- `app.js` – jQuery event handlers, DOM operations, animations, AJAX requests, and error handling.
- `students.json` – Mock student data used by the AJAX examples.

---

## ▶️ Run the Experiment

Serve the folder through a local web server so that the AJAX requests can load `students.json` correctly.

From the `Experiment 10` folder, run:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser.

Click the Program 1 buttons to test DOM effects. In Program 2, use the AJAX buttons to load the student data or simulate a failed request.

---

## 📌 Conclusion

This experiment demonstrates how jQuery simplifies browser-side development. It covers selectors, event handling, DOM updates, animations, asynchronous JSON retrieval, and practical error handling through `$.ajax()` and `$.getJSON()`.
