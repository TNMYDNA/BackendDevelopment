# Lab Examination — MongoDB Notes Application

**SAP ID:** 590014609

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

Open [http://localhost:3000](http://localhost:3000) in a browser.

## Routes

- `GET /` — display all notes.
- `POST /notes` — create a note.
- `POST /notes/:id/delete` — delete a note.

Notes are stored in the `notes_lab` database and the `notes` collection.
