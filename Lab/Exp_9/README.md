# Experiment 9: Asynchronous Data Exchange Using AJAX

**Course:** Backend Development  
**(SAP:- 590014609)**

---

## 🎯 Aim & Objectives

### Aim
To understand asynchronous data exchange in web applications using AJAX and the modern Fetch API, and to retrieve and display JSON, XML, and HTML data without reloading the page.

### Key Objectives
1. **AJAX and Fetch API**: Make asynchronous HTTP requests from the browser using `fetch()`.
2. **JSON Processing**: Retrieve a JSON document, parse it, and display student records in a table.
3. **XML Processing**: Retrieve XML data, parse it with `DOMParser`, and convert it into JavaScript objects.
4. **HTML Fragments**: Fetch an HTML fragment and insert it dynamically into the current page.
5. **DOM Manipulation**: Update tables, messages, and content containers based on the response received.
6. **Error Handling**: Check HTTP responses and display loading, success, and error messages.

---

## 📚 Theoretical Background

### AJAX
AJAX (Asynchronous JavaScript and XML) allows a web page to communicate with a server asynchronously. The page can request data and update only the required section without performing a full reload.

### Fetch API
The Fetch API provides a promise-based interface for making HTTP requests. A response can be converted into the required format with methods such as `response.json()` and `response.text()`.

### JSON and XML
- **JSON** is parsed using `response.json()` and is convenient for structured application data.
- **XML** is received as text and parsed with `DOMParser` before values are read from the XML document.

### DOM Updates
JavaScript creates table rows and cells dynamically, changes element visibility, inserts HTML content, and updates status messages in response to user actions.

---

## 💻 Application Features

1. **Fetch JSON Students**: Loads `students.json` and displays student records in a table.
2. **Fetch XML Students**: Loads `students.xml`, parses each `<student>` element, and displays the records in the same table.
3. **Fetch HTML Notice**: Loads `notice.html` and inserts the returned HTML fragment into the page.
4. **Request Status**: Shows loading, success, and failure messages for each asynchronous request.
5. **Responsive Interface**: Provides a styled interface with separate controls for each data format.

---

## 📁 Files

- `index.html` – Page layout, buttons, status area, and student table.
- `app.js` – Fetch requests, JSON/XML parsing, DOM updates, and error handling.
- `students.json` – Student records in JSON format.
- `students.xml` – Student records in XML format.
- `notice.html` – HTML fragment loaded dynamically through Fetch.
- `style.css` – Application styling and response-state styles.

---

## ▶️ Run the Experiment

Because the application uses `fetch()`, serve the folder through a local web server instead of opening `index.html` directly.

From the `Exp_9` folder, run:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser and select any button to load the corresponding data format.

---

## 📌 Conclusion

This experiment demonstrates how AJAX and the Fetch API can retrieve JSON, XML, and HTML asynchronously. The application parses each response, updates the page dynamically through DOM manipulation, and handles loading and error states without refreshing the browser.
