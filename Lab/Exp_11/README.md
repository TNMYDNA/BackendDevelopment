# Experiment 11: Asynchronous Student and Course Portal

**Course:** Backend Development  
**(SAP:- 590014609)**

---

## 🎯 Aim & Objectives

### Aim
To build a browser-based academic portal using HTML5, CSS3, modern JavaScript, AJAX Fetch API, JSON, XML, and client-side filtering.

### Key Objectives
1. **Asynchronous Data Loading**: Fetch student and course data without reloading the page.
2. **JSON and XML Support**: Load JSON using `response.json()` and XML using `DOMParser`.
3. **Dynamic Rendering**: Generate student table rows and course cards from fetched data.
4. **Search and Filtering**: Filter students by name, ID, email, and course.
5. **Statistics**: Calculate total records, average GPA, and active enrollments.
6. **Single-Page Navigation**: Switch between student, course, and architecture views using tabs.
7. **Error Handling**: Display useful status messages when requests succeed or fail.

---

## 📚 Theoretical Background

### AJAX and Fetch API
AJAX allows a web page to exchange data with a server asynchronously. The Fetch API provides a promise-based way to request resources and process HTTP responses without refreshing the page.

### JSON and XML Parsing
- **JSON** is converted into JavaScript objects with `response.json()`.
- **XML** is read as text and converted into a document using `DOMParser`.

### DOM Manipulation
JavaScript creates table rows and course cards dynamically, changes status messages, updates statistics, and controls the visibility of tab panels.

### Client-Side Filtering
After the student data is loaded, search and course filters operate on the in-memory array. This provides immediate results without sending a new request for every filter action.

### Single-Page Architecture
The application separates its presentation from its data sources. The interface loads immediately, while JSON and XML payloads are fetched only when needed.

---

## 💻 Practice Tasks

1. **Student Directory**: Load student records from JSON and display them in a table.
2. **XML Data Source**: Switch to the XML source and parse student elements with `DOMParser`.
3. **Search and Course Filter**: Search by student name, ID, or email and filter by course.
4. **Statistics Bar**: Display total records, average GPA, and active enrollment count.
5. **Course Catalog**: Load `courses.json` when the Courses Catalog tab is opened and render course cards.
6. **Refresh Data**: Reload the currently selected student data source asynchronously.

---

## 📁 Files

- `index.html` – Portal layout, navigation tabs, filters, statistics, tables, and course area.
- `app.js` – Fetch requests, JSON/XML parsing, filtering, statistics, tab navigation, and rendering logic.
- `style.css` – Portal styling, cards, tables, controls, and status messages.
- `students.json` – Student records in JSON format.
- `students.xml` – Student records in XML format.
- `courses.json` – Course catalog data loaded on demand.

---

## ▶️ Run the Experiment

Serve the folder through a local web server so the Fetch API can load the JSON and XML files.

From the `Exp_11` folder, run:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser. Use the tabs to switch views, select JSON or XML, search for students, filter by course, and load the course catalog.

---

## 📌 Conclusion

This experiment demonstrates a decoupled single-page academic portal that retrieves JSON and XML asynchronously, processes data in the browser, updates the DOM dynamically, and provides interactive search, filtering, statistics, and course browsing features.
