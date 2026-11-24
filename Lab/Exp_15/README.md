# Experiment 15 — Django To-Do Application

**SAP ID:** 590014609

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
