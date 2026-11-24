# Lecture 14 — Database Design and Normalization

**SAP ID:** 590014609

This lecture covers relational schema design, entity relationships, normalization, primary keys, foreign keys, and junction tables.

## Library management system

- `library_er_diagram.md` — entities and relationships for authors, books, members, and loans.
- `library_schema_design.md` — detailed table and relationship definitions.
- `library_schema.sql` — SQL statements that create the normalized library schema.

The library schema includes:

- `Author` and `Book` with a many-to-many relationship through `Book_Author`.
- `Member` and `Loan` with a one-to-many relationship.
- `Book` and `Loan` with a one-to-many relationship.

## Order normalization

- `order_normalization.md` — works through first, second, and third normal forms.
- `normalized_orders.sql` — creates and populates the final 3NF schema.

The normalized order design separates data into:

- `Customers`
- `Orders`
- `Products`
- `Order_Details`

## Run the SQL examples

Use a PostgreSQL database or another compatible relational database, then execute the scripts with your database client. For PostgreSQL:

```bash
psql your_database -f library_schema.sql
psql your_database -f normalized_orders.sql
```

The scripts demonstrate how primary keys, foreign keys, unique constraints, and composite keys preserve data integrity while reducing duplication.
