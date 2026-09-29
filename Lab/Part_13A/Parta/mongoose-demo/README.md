# Experiment 13 Part A: MongoDB, Mongoose, and Express User Registration and Login System

**Course:** Backend Development  
**(SAP:- 590014609)**

---

## 🎯 Aim & Objectives

### Aim
To learn and implement MongoDB database connectivity using the Mongoose ODM in an Express.js web application, building a full user registration and authentication system with schema validation, unique indexes, password hashing (`bcrypt`), and asynchronous database queries (`find`, `findOne`, `save`).

### Key Objectives
1. **Database Connectivity**: Connect Express application to local MongoDB / MongoDB Atlas using `mongoose.connect()`.
2. **Schema & Model Definition**: Define structured database blueprints with `mongoose.Schema` enforcing field types, `required`, `unique`, and `default` values.
3. **Password Security**: Hash passwords securely prior to database storage using `bcrypt.hash()` and verify incoming credentials with `bcrypt.compare()`.
4. **CRUD Operations**: Perform asynchronous database operations using `save()`, `findOne()`, and `find()`.
5. **Duplicate & Validation Error Handling**: Handle MongoDB duplicate key errors (code `11000`) and schema validation errors gracefully.

---

## 📚 Theoretical Background

### MongoDB & Document Databases
MongoDB is a NoSQL, document-oriented database that stores data in flexible, JSON-like BSON documents. Unlike relational SQL databases, documents do not require fixed tables or complex multi-table joins.

### Mongoose ODM
Mongoose is an Object Data Modeling (ODM) library for Node.js. It manages relationships between data, provides schema validation, and translates between JavaScript code objects and MongoDB database documents.

- **Schema**: Defines the structural blueprint (keys, types, defaults, validation rules).
- **Model**: A constructor compiled from a Schema that interfaces directly with database collections.
- **Document**: An individual instance of a Model corresponding to a single MongoDB document.

### Password Security & Hashing (`bcrypt`)
Storing plain-text passwords is a major security flaw. `bcrypt` applies a cryptographic salt and hash algorithm to passwords before saving them to MongoDB, ensuring plain-text credentials are never exposed even if the database is compromised.

---

## 💻 Practice Tasks

1. **MongoDB Connection Setup**: Configure Mongoose connection handling with success and error promises (`.then()` / `.catch()`).
2. **User Schema & Model Creation**: Build a user schema with string trimming, required constraints, and unique indexes for `username` and `email`.
3. **Secure User Registration (`/signup`)**: Parse registration form submissions, validate password rules, hash passwords using `bcrypt`, and handle duplicate key errors.
4. **Credential Verification (`/login`)**: Locate user records asynchronously by username and verify password hashes.
5. **Registered Users Listing (`/users`)**: Query and render all database user documents sorted by registration date.

---

## 📌 Conclusion

In this experiment, an Express web application was integrated with MongoDB using the Mongoose ODM. The lab demonstrated database connection setup, Schema and Model creation, asynchronous document querying and saving, `bcrypt` password hashing, unique index constraint enforcement, and user authentication workflows.
