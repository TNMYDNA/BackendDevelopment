# Lecture 5 — FastAPI CRUD and API Documentation

**SAP ID:** 590014609

This lecture introduces FastAPI through in-memory CRUD APIs, query filtering, request validation with Pydantic, and automatically generated API documentation.

## Examples

- `Task-1-FastAPI-CRUD.py` — Student Management API with list, retrieve, create, update, delete, and branch-filtering endpoints.
- `Lab Exercise/Task-1-Course-API.py` — Course Management API with department filtering and full CRUD operations.
- `Task-1-Swagger.png` — Swagger UI documentation example.
- `Lab Exercise/Lab-Exercise-3-Swagger.png` — Swagger UI exercise result.
- `Lab Exercise/Lab-Exercise-4-ReDoc.png` — ReDoc documentation example.
- `Lab Exercise/Lab-Exercise-5-Department-Filter.png` — Department-filtering result.

## Installation

Install the required Python packages:

```bash
python -m pip install fastapi uvicorn pydantic
```

## Run an API

From this directory, start either application with Uvicorn:

```bash
uvicorn Task-1-FastAPI-CRUD:app --reload --port 5000
```

For the course API:

```bash
uvicorn "Lab Exercise.Task-1-Course-API:app" --reload --port 5001
```

The student API is available at [http://127.0.0.1:5000](http://127.0.0.1:5000), and the course API at [http://127.0.0.1:5001](http://127.0.0.1:5001).

## API documentation

FastAPI generates interactive documentation automatically:

- Swagger UI: `/docs`
- ReDoc: `/redoc`

For example, open [http://127.0.0.1:5000/docs](http://127.0.0.1:5000/docs) after starting the student API.
