# Lecture 6 — Sessions, Cookies, and Query Strings

**SAP ID:** 590014609

This lecture demonstrates common ways to maintain user state and read client-supplied values in Express.js applications.

## Examples

- `Task-1-Sessions.js` — starts a session, displays a profile, and logs the user out using `express-session`.
- `Task-2-Cookies.js` — sets, reads, and deletes a cookie using `cookie-parser`.
- `Task-3-Query-Strings.js` — reads `user` and `role` values from a URL query string.

## Installation

From this directory, install the required packages:

```bash
npm init -y
npm install express express-session cookie-parser
```

## Run an example

Start one script at a time:

```bash
node Task-1-Sessions.js
```

The examples listen on port `3000`. Stop the running server before starting another example.

## Routes

### Sessions

- `GET /login` — starts a session for `JohnDoe`.
- `GET /profile` — displays the active session user.
- `GET /logout` — destroys the session.

### Cookies

- `GET /setcookie` — creates a username cookie.
- `GET /getcookie` — reads the username cookie.
- `GET /deletecookie` — removes the cookie.

### Query strings

Open the following URL after starting `Task-3-Query-Strings.js`:

```text
http://localhost:3000/welcome?user=Aarav&role=student
```
