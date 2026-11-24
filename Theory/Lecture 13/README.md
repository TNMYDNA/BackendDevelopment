# Lecture 13 — Relational and NoSQL Databases

**SAP ID:** 590014609

This lecture introduces database fundamentals by comparing PostgreSQL, a relational database, with MongoDB, a NoSQL document database. The examples use the same student-management scenario in both systems.

## Files

- `student_management.sql` — PostgreSQL database, table, insert, select, update, and delete operations.
- `mongodb_students.js` — MongoDB collection creation, document insertion, and student queries.
- `postgresql-quick-reference.md` — PostgreSQL command-line reference.
- `sql-vs-mongodb.md` — space for SQL and MongoDB comparison notes.

## PostgreSQL example

Create the database and open it with `psql`:

```bash
createdb student_management
psql student_management
```

Run the contents of `student_management.sql` in the PostgreSQL client:

```bash
psql student_management -f student_management.sql
```

The script creates a `students` table and demonstrates filtering CSE students, querying enrollment dates, updating a branch, and deleting a record.

## MongoDB example

Open the MongoDB shell and run the script:

```bash
mongosh
load("mongodb_students.js")
```

The script uses the `student_management` database, inserts three student documents into the `students` collection, and queries students by branch and enrollment date.

## Key difference

PostgreSQL stores structured rows in tables with a defined schema. MongoDB stores flexible JSON-like documents in collections. Both examples implement similar student queries using their respective query languages.
