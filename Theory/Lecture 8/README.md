---
layout: default
title: Lecture 8 — Server-Side Rendering and Static Content
permalink: /Theory/Lecture%208/
---

# Lecture 8 — Server-Side Rendering and Static Content

**SAP ID:** 590014609

This lecture compares server-side rendering approaches in Node.js and Python, and demonstrates how Express serves static assets alongside rendered views.

## Sections

- **Part B — Node, Express, and EJS:** Renders home and student pages with EJS templates.
- **Part C — FastAPI and Jinja2:** Renders a student table with Jinja2 templates.
- **Part D — Express Static Content:** Serves files from a `public` directory and renders a student list with EJS.

## Node.js SSR example

From `Part-B-Node-Express-EJS/ssr-demo`, install dependencies and start the server:

```bash
npm install
npm start
```

Open 'http://localhost:3000' for the home page or 'http://localhost:3000/students' for the rendered student list.

## FastAPI and Jinja2 example

From `Part-C-FastAPI-Jinja2/ssr-python`, install the Python dependencies and run the application:

```bash
python -m pip install fastapi uvicorn jinja2
python main.py
```

Open 'http://127.0.0.1:8000' to view the rendered page.

## Static-content example

From `Part-D-Static-Content/express-static-demo`, install the dependencies and start the app:

```bash
npm install
node app.js
```

Open 'http://localhost:3000/students' to view the EJS-rendered student list. Files placed in the `public` directory are served as static content.
