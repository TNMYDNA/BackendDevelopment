# Lecture 15 — ORM, MongoDB, and Data Validation

**SAP ID:** 590014609

This lecture demonstrates relational data modeling with SQLAlchemy, conceptual e-commerce modeling, MongoDB document relationships with Mongoose, and request validation with FastAPI and Pydantic.

## Tasks

- **Task 1 — Data Modeling:** `Task1_Data_Modeling/model.py` defines Department, Student, Course, and Enrollment models with SQLAlchemy and stores them in SQLite.
- **Task 2 — E-commerce Model:** `Task2_Ecommerce_Model/` describes customers, carts, products, and orders using a Mermaid diagram and relationship notes.
- **Task 3 — Mongoose Blog:** `Task3_Mongoose_Blog/app.js` creates posts and comments in MongoDB and uses `populate()` to read related posts.
- **Task 4 — Data Validation:** `Task4_Data_Validation/app.py` validates student data with Pydantic before storing it through a FastAPI endpoint.

## Run the SQLAlchemy example

From `Task1_Data_Modeling`:

```bash
python -m pip install sqlalchemy
python model.py
```

This creates or updates the local `students.db` SQLite database and demonstrates create, read, update, and delete operations.

## Run the Mongoose example

Start a local MongoDB server, then from `Task3_Mongoose_Blog` install dependencies and run the script:

```bash
npm install
node app.js
```

The script connects to `mongodb://127.0.0.1:27017/blog_database`.

## Run the validation API

From `Task4_Data_Validation`:

```bash
python -m pip install "fastapi[email]" uvicorn
uvicorn app:app --reload
```

The `POST /students` endpoint validates names, email addresses, branches, and enrollment dates. Interactive documentation is available at [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs).
