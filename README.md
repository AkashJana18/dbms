<p><a target="_blank" href="https://app.eraser.io/workspace/SoAZWqIyNfuLnfJG69BC" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

# Introduction of DBMS (Database Management System)
A **database **is a collection of interrelated data that helps in the efficient retrieval, insertion, and deletion of data from the database and organizes the data in the form of tables, views, schemas, reports, etc. **For Example**, a university database organizes the data about students, faculty, admin staff, etc. which helps in the efficient retrieval, insertion, and deletion of data from it.

## What is DBMS?
A Database Management System (DBMS) is a software system that is designed to manage and organize data in a structured manner. It allows users to create, modify, and query a database, as well as manage the security and access controls for that database. DBMS provides an environment to store and retrieve data in convenient and efficient manner

**DBMS can be classified into two types:**

![Figure 1](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---ucdXHkmSCswShjJt3fdHs---figure---ta711QFKI1XLSLh4ZMH9fg.png "Figure 1")

- **RDBMS: **Data is organized in the form of tables and each table has a set of rows and columns. The data are related to each other through primary and foreign keys.
- **NoSQL: **Data is organized in the form of key-value pairs, documents, graphs, or column-based. These are designed to handle large-scale, high-performance scenarios.
- **Object-Oriented DBMS (OODBMS):** Stores data as objects, similar to those used in object-oriented programming, allowing for complex data representations and relationships
### Key Features of DBMS:
![Figure 3](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---fBYoLTeByaQVJhSBFDuSI---figure---vziU3Rlwqb9_xWOy3myXgA.png "Figure 3")

# Database Languages
![Figure 4](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---EYXnvmYMbat5_IJMVwxxh---figure---FMkNCcuqFYeHLCABzV6kJg.png "Figure 4")

## Data Definition Language (DDL)
**DDL** is the short name for Data Definition Language, which deals with database schemas and descriptions, of how the data should reside in the database.

## Data Manipulation Language (DML)
**DML** is the short name for Data Manipulation Language which deals with data manipulation and includes most common SQL statements such SELECT, INSERT, UPDATE, DELETE, etc., and it is used to store, modify, retrieve, delete and update data in a database. 

## Data Control Language (DCL)
**DCL **is short for Data Control Language which acts as an access specifier to the database.(basically to grant and revoke permissions to users in the database.

## Transactional Control Language (TCL)
**TCL** is short for Transactional Control Language which acts as an manager for all types of transactional data and all transactions.

## Data Query Language (DQL)
**Data query language(DQL)** is the subset of **“Data Manipulation Language”**. The most common command of DQL is 1the **SELECT statement**. SELECT statement helps us in retrieving the data from the table without changing anything or modifying the table. DQL is very important for retrieval of essential data from a database.

```markdown
| **Category**                        | **Commands**                                                                                       | **Description**                                                                                                      |
|-------------------------------------|----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **Data Definition Language (DDL)**  | CREATE                                                                                            | Create a database and its objects like tables, indexes, views, stored procedures, functions, and triggers.           |
|                                     | ALTER                                                                                             | Alters the structure of the existing database.                                                                       |
|                                     | DROP                                                                                              | Deletes objects from the database.                                                                                   |
|                                     | TRUNCATE                                                                                          | Removes all records from a table and frees the space allocated for the records.                                       |
|                                     | COMMENT                                                                                           | Adds comments to the data dictionary.                                                                                |
|                                     | RENAME                                                                                            | Renames an object.                                                                                                   |
| **Data Manipulation Language (DML)**| SELECT                                                                                            | Retrieves data from a database.                                                                                      |
|                                     | INSERT                                                                                            | Inserts data into a table.                                                                                           |
|                                     | UPDATE                                                                                            | Updates existing data within a table.                                                                                |
|                                     | DELETE                                                                                            | Deletes records from a database table.                                                                               |
|                                     | MERGE                                                                                             | Performs UPSERT operation (insert or update).                                                                        |
|                                     | CALL                                                                                              | Calls a PL/SQL or Java subprogram.                                                                                   |
|                                     | EXPLAIN PLAN                                                                                      | Displays the execution plan for a SQL query.                                                                         |
|                                     | LOCK TABLE                                                                                        | Controls concurrency by locking tables.                                                                              |
| **Data Control Language (DCL)**     | GRANT                                                                                             | Grants permissions to users for running DML commands on a table.                                                     |
|                                     | REVOKE                                                                                            | Revokes permissions from users for running DML commands on a table.                                                  |
| **Transactional Control Language (TCL)** | ROLLBACK                                                                                        | Cancels or undoes changes made to the database.                                                                      |
|                                     | COMMIT                                                                                            | Saves changes made to the database permanently.                                                                      |
|                                     | SAVEPOINT                                                                                         | Sets a savepoint to save the current state of the database transaction temporarily.                                   |
```




<!--- Eraser file: https://app.eraser.io/workspace/SoAZWqIyNfuLnfJG69BC --->