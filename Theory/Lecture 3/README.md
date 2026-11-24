# Lecture 3 — Backend Routes and Responses

**SAP ID:** 590014609

This lecture contains introductory examples using Express.js and Flask. The examples progress from a basic server to multiple routes, JSON data, HTML responses, templates, and POST requests.

## Topics and tasks

1. **Task 1 — Hello World:** Start a basic Express server.
2. **Task 2 — Multiple Routes:** Add student-management routes.
3. **Task 3 — JSON Data:** Return students as JSON and filter by branch or ID.
4. **Task 4 — HTML Responses:** Generate HTML responses for student data.
5. **Task 5 — EJS Templating:** Render student pages with EJS views.
6. **Task 6 — Flask Hello World:** Start a basic Flask server.
7. **Task 7 — Flask Routes, JSON, and POST:** Read, create, and retrieve students through Flask routes.
8. **Task 8 — DevTools:** Inspect requests and responses using browser developer tools.

## Run the Express examples

From the selected task directory, install the required packages and start the server:

```bash
npm init -y
npm install express
node server.js
```

For Task 5, install EJS as well:

```bash
npm install express ejs
```

The servers run on [http://localhost:3000](http://localhost:3000).

## Run the Flask examples

Install Flask and start the application from the selected task directory:

```bash
python -m pip install flask
python app.py
```

The Flask development server is available at [http://127.0.0.1:5000](http://127.0.0.1:5000).
