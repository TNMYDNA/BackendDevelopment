---
layout: default
title: Lecture 26 — Django Student Management API
permalink: /Theory/Lecture%2026/
---

# Lecture 26 — Django Student Management API

**SAP ID:** 590014609

This lecture contains a minimal Django project that exposes a JSON welcome endpoint for a student management system.

## Project structure

- `student_system/manage.py` — Django command-line entry point.
- `student_system/student_system/` — project settings, URL configuration, and WSGI/ASGI setup.
- `student_system/students/` — the students application, including its view and future model/admin files.

## Installation

From the `student_system` directory, install Django:

```bash
python -m pip install django
```

## Run the development server

```bash
python manage.py migrate
python manage.py runserver
```

Open 'http://127.0.0.1:8000/'. The root endpoint returns a JSON response containing the API message, version, and running status.

The Django admin is available at 'http://127.0.0.1:8000/admin/' after creating a superuser:

```bash
python manage.py createsuperuser
```

## API endpoint

| Method | Endpoint | Description |
| --- | --- | --- |
| `GET` | `/` | Returns the Student Management API status as JSON. |
