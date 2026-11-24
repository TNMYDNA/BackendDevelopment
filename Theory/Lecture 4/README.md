# Lecture 4 — API Testing and HTTP Requests

This lecture demonstrates how to test backend APIs and inspect HTTP requests using browser developer tools, `curl`, Postman, and JavaScript's `fetch` API.

## Exercises

- **Exercise 1:** Inspect API requests with browser DevTools.
- **Exercise 2:** Test API endpoints from the command line with `curl`.
- **Exercise 3:** Send requests and inspect responses with Postman.
- **Exercise 4:** Compare browser DevTools and Postman while testing APIs.
- **Exercise 5:** Use verbose `curl` output and Postman to inspect request details.

The screenshots in this folder show the completed requests and responses for each exercise.

## Fetch example

The `Lab Exercise 4/fetch-students.js` file requests students from a local API and filters the response to only CSE students:

```bash
node "Lab Exercise 4/fetch-students.js"
```

The API must be running at `http://localhost:3000/students` before executing the script. The endpoint should return a JSON array of student objects containing a `branch` field.

## Useful commands

```bash
# Make a basic GET request
curl http://localhost:3000/students

# Display request and response details
curl -v http://localhost:3000/students
```

Postman can be used for the same endpoints when a graphical interface is preferred.
