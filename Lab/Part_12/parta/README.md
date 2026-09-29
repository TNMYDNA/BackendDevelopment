# Experiment 12 Part A: Node.js, Express.js, Nodemon, and EJS Templating

**Course:** Backend Development  
**(SAP:- 590014609)**

---

## 🎯 Aim & Objectives

### Aim
To understand and implement server-side JavaScript using Node.js, build RESTful HTTP APIs using Express.js, process route parameters and POST form submissions, render dynamic web pages using EJS templating, and utilize development tools such as Nodemon.

### Key Objectives
1. **Node.js & NPM Setup**: Initialize Node.js projects, manage `package.json`, and handle dependencies.
2. **Express Server & Routing**: Build web servers with Express handling GET/POST requests, route parameters (`req.params`), query strings (`req.query`), and status codes.
3. **Response Formats**: Deliver plain text, structured JSON responses, and HTML views.
4. **EJS Templating**: Render dynamic views (`<%= %>`, `<% %>`) passing backend data to template engine templates.
5. **Form Handling**: Handle POST submissions using `express.urlencoded()` and `express.json()`.
6. **Development Tooling**: Configure `nodemon` for auto-restarting local development servers on code modifications.

---

## 📚 Theoretical Background

### Node.js & NPM
Node.js is an event-driven, asynchronous I/O JavaScript runtime built on Google Chrome's V8 engine. NPM (Node Package Manager) manages project dependencies via `package.json`.

### Express.js Framework
Express is a minimalist web framework providing simplified routing (`app.get()`, `app.post()`), middleware chaining (`app.use()`), and template rendering (`res.render()`).

### Response Types
- `res.send()`: Sends text or HTML buffers.
- `res.json()`: Sends JSON with proper `Content-Type: application/json` headers.
- `res.render()`: Compiles and outputs EJS views with dynamic data contexts.

### EJS & Nodemon
- **EJS**: Embedded JavaScript templates allowing conditional logic, loops (`forEach`), and variable output directly inside HTML.
- **Nodemon**: File watcher that restarts the Node process automatically upon script edits.

---

## 💻 Practice Tasks

1. **Basic Server Routes**: Implement routes returning text, HTML, and JSON data.
2. **Calculator API**: Build a calculator API endpoint handling `add`, `subtract`, `multiply`, and `divide` via query parameters.
3. **Student Management API**: Implement GET and POST endpoints for retrieving and adding student records.
4. **EJS Course Timetable**: Create an EJS template to display a weekly course timetable dynamically passed from Express.
5. **Form Submission & Results Page**: Create an EJS student registration form and render the submitted data on a results page.

---

## 📌 Conclusion

In this experiment, a complete Node.js web application was built using Express.js and EJS. The lab demonstrated setting up NPM dependencies, handling GET/POST requests, parsing route parameters and query strings, rendering dynamic EJS templates, and automating development workflows with Nodemon.
