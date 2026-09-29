# Experiment 12 Part B: Session & Cookie State Management in Node.js

**Course:** Backend Development  
**(SAP:- 590014609)**


---

## 🎯 Aim & Objectives

### Aim
To understand the stateless nature of HTTP and implement client-side (cookies) and server-side (sessions) state management mechanisms in a Node.js/Express web application for user authentication and session-specific data persistence.

### Key Objectives
1. **Stateless Protocol Awareness**: Comprehend why state management is necessary over HTTP.
2. **Cookie Management**: Set, retrieve, and clear client-side HTTP cookies using `cookie-parser` with `HttpOnly` and `maxAge` security flags.
3. **Session Management**: Implement server-side session tracking using `express-session` with secret keys, session stores, and session expiration.
4. **Authentication & Authorization**: Protect sensitive routes using custom authentication middleware (`authMiddleware`).
5. **Session Data Persistence**: Build session-scoped interactive components (e.g., a per-session To-Do list manager).

---

## 📚 Theoretical Background

### Why HTTP is Stateless
HTTP is a stateless protocol; every request sent from a client to a server is treated independently. Without state management, web servers cannot natively recognize whether sequential requests come from the same user.

### Cookies vs. Sessions

| Feature | Cookie | Session |
|---------|--------|---------|
| **Storage Location** | Client Browser | Server Memory / Database |
| **Data Capacity** | Small (~4KB max) | Large (Server capacity limit) |
| **Security** | Visible to user (unless `HttpOnly`) | Highly Secure (Sensitive data stays on server) |
| **Ideal For** | User preferences, theme, UI state | Authentication, user IDs, shopping carts |

### How Sessions & Cookies Work Together
1. User logs in with credentials.
2. Server validates user and initializes a session object (`req.session.user`).
3. Server generates a unique Session ID and sends it back to the client as an `HttpOnly` cookie (`connect.sid`).
4. Subsequent requests automatically include the `connect.sid` cookie, enabling the server to look up the active session.
5. On logout, the server calls `req.session.destroy()` and clears the cookie via `res.clearCookie()`.

---

## 💻 Practice Tasks

1. **Simple User Login & Session Auth**: Build a registration and login system that stores user sessions upon successful login and redirects unauthorized requests.
2. **Protected Dashboard Route**: Implement middleware that verifies active sessions before allowing access to private routes.
3. **Session-based To-Do List**: Create a To-Do list manager where items are stored per user session (`req.session.todos`).
4. **Cookie Preference Setting**: Store user theme settings in a cookie and apply the preference across requests.

---

## 📌 Conclusion

In this experiment, session and cookie management mechanisms were successfully implemented using Node.js, Express, `express-session`, and `cookie-parser`. The lab demonstrated handling user authentication sessions, implementing route authorization middleware, managing client-side cookies securely, and storing per-session interactive data.
