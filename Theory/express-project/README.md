# Express Project

A small Express.js server with a welcome route and a sample students API.

## Requirements

- Node.js 18 or newer
- npm

## Installation

From this directory, install the dependencies:

```bash
npm install
```

## Run the server

Start the application with:

```bash
npm start
```

The server listens on port `3000`. Open [http://localhost:3000](http://localhost:3000).

For development with automatic restarts, run:

```bash
npm run dev
```

## API endpoints

| Method | Endpoint | Description |
| --- | --- | --- |
| `GET` | `/` | Returns a welcome message. |
| `GET` | `/api/students` | Returns a JSON list of sample students. |

Example:

```bash
curl http://localhost:3000/api/students
```
