# Experiment 15 — Django To-Do Application

**SAP ID:** 590014609

**Course:** Backend Development

---

## 🎯 Aim & Objectives

### Aim
To build a Django to-do application using models, migrations, templates, static files, and database-backed CRUD operations.

### Key Objectives
1. Create a Django project and application.
2. Define a `Task` model with status and timestamps.
3. Apply migrations and use SQLite through the Django ORM.
4. Render task data with Django templates.
5. Implement add, toggle, and delete actions.

---

## 📚 Theoretical Background

Django follows a Model-View-Template architecture. Models describe database records, views process requests and coordinate application logic, and templates render HTML responses. Migrations keep the database schema synchronized with model definitions.

This experiment is a Django-based to-do application that demonstrates models, migrations, templates, static files, and CRUD-style task actions.

## Features

- View tasks sorted by creation time.
- Add a new task.
- Mark tasks complete or incomplete.
- Delete tasks.
- Store task data in SQLite through Django's ORM.
- Use Django templates and static CSS styling.

## Requirements

- Python 3.10 or newer
- Django 4.2 or newer

## Setup

From the `Lab/Exp_15` directory, install Django and apply migrations:

```bash
python -m pip install django
python manage.py migrate
```

For a non-development environment, set a strong secret key before starting the application:

```bash
export DJANGO_SECRET_KEY="your-secret-key"
```

## Run the application

```bash
python manage.py runserver
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) to view the task list.

## Routes

- `/` — display all tasks.
- `/add/` — add a task.
- `/toggle/<task_id>/` — toggle completion status.
- `/delete/<task_id>/` — delete a task.
- `/admin/` — Django administration interface.

---

## 💻 Practice Tasks

1. Create the Django project and `todo` application.
2. Define and migrate the `Task` model.
3. Display tasks ordered by creation time.
4. Add new tasks through a form.
5. Toggle completion status.
6. Delete tasks and verify the updated list.

---

## 📌 Conclusion

This experiment demonstrates a complete Django CRUD workflow with database persistence, server-rendered templates, static styling, and reusable URL patterns.
