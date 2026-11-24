# Lab Examination — MongoDB Notes Application

**SAP ID:** 590014609

**Course:** Backend Development

---

## 🎯 Aim & Objectives

### Aim
To build a full-stack notes application using Express.js, MongoDB, the native MongoDB driver, and EJS server-side rendering.

### Key Objectives
1. Connect an Express application to MongoDB.
2. Insert and retrieve note documents.
3. Validate form input before saving data.
4. Delete documents using MongoDB `ObjectId` values.
5. Render database records with EJS templates.

---

## 📚 Theoretical Background

MongoDB stores flexible document-oriented data in collections. Express handles HTTP routes and middleware, while EJS generates HTML from server-side data. Together, these technologies provide a simple full-stack workflow for creating, reading, and deleting notes.

This project is an Express.js notes application that uses MongoDB for persistent storage and EJS for server-side rendering.

## Features

- Add notes with a title, content, and category.
- Display all saved notes.
- Delete notes by MongoDB ObjectId.
- Render pages with EJS templates.
- Serve CSS from the `public` directory.

## Requirements

- Node.js 18 or newer
- npm
- MongoDB running locally on port `27017`

## Setup

From this directory, install the dependencies:

```bash
npm install
```

The application connects to MongoDB at:

```text
mongodb://127.0.0.1:27017/notes_lab
```

## Run the application

```bash
node server.js
```

While the server is running, enter `http://localhost:3000` in your browser.

## Routes

- `GET /` — display all notes.
- `POST /notes` — create a note.
- `POST /notes/:id/delete` — delete a note.

Notes are stored in the `notes_lab` database and the `notes` collection.

---

## 💻 Practice Tasks

1. Connect to a local MongoDB server.
2. Create the `notes_lab` database and `notes` collection.
3. Submit and validate a new note.
4. Display all saved notes in an EJS view.
5. Delete a note by its ObjectId.
6. Serve the application stylesheet from the `public` directory.

---

## 📌 Conclusion

This examination project combines Express routing, MongoDB persistence, form handling, EJS templating, and static content serving in one working notes application.
