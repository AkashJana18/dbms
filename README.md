<p><a target="_blank" href="https://app.eraser.io/workspace/SoAZWqIyNfuLnfJG69BC" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

# Introduction of DBMS (Database Management System)
A **database **is a collection of interrelated data that helps in the efficient retrieval, insertion, and deletion of data from the database and organizes the data in the form of tables, views, schemas, reports, etc. **For Example**, a university database organizes the data about students, faculty, admin staff, etc. which helps in the efficient retrieval, insertion, and deletion of data from it.

## What is DBMS?
A Database Management System (DBMS) is a software system that is designed to manage and organize data in a structured manner. It allows users to create, modify, and query a database, as well as manage the security and access controls for that database. DBMS provides an environment to store and retrieve data in convenient and efficient manner

**DBMS can be classified into two types:**

![Figure 1](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---yi-GYJaiNlXZrSrL_7W6j---figure---ta711QFKI1XLSLh4ZMH9fg.png "Figure 1")

- **RDBMS: **Data is organized in the form of tables and each table has a set of rows and columns. The data are related to each other through primary and foreign keys.
- **NoSQL: **Data is organized in the form of key-value pairs, documents, graphs, or column-based. These are designed to handle large-scale, high-performance scenarios.
- **Object-Oriented DBMS (OODBMS):** Stores data as objects, similar to those used in object-oriented programming, allowing for complex data representations and relationships
### Key Features of DBMS:
![Figure 3](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---N3uJDqODd5FNLXIh45EUM---figure---vziU3Rlwqb9_xWOy3myXgA.png "Figure 3")

# Database Languages
![Figure 4](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---G0vUnEWt6CHdWobi_0mff---figure---FMkNCcuqFYeHLCABzV6kJg.png "Figure 4")

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

## SQL Commands Overview
### Data Definition Language (DDL)
- **CREATE**: Create a database and its objects like tables, indexes, views, stored procedures, functions, and triggers. 
- **ALTER**: Alters the structure of the existing database. 
- **DROP**: Deletes objects from the database.
- **TRUNCATE**: Removes all records from a table and frees the space allocated for the records. 
- **COMMENT**: Adds comments to the data dictionary. - **RENAME**: Renames an object.
### Data Manipulation Language (DML)
- **SELECT**: Retrieves data from a database.
- **INSERT**: Inserts data into a table.
- **UPDATE**: Updates existing data within a table.
- **DELETE**: Deletes records from a database table.
- **MERGE**: Performs UPSERT operation (insert or update).
- **CALL**: Calls a PL/SQL or Java subprogram.
- **EXPLAIN PLAN**: Displays the execution plan for a SQL query.
- **LOCK TABLE**: Controls concurrency by locking tables.
### Data Control Language (DCL)
- **GRANT**: Grants permissions to users for running DML commands on a table.
- **REVOKE**: Revokes permissions from users for running DML commands on a table.
### Transactional Control Language (TCL)
- **ROLLBACK**: Cancels or undoes changes made to the database.
- **COMMIT**: Saves changes made to the database permanently.
- **SAVEPOINT**: Sets a savepoint to save the current state of the database transaction temporarily.
# Paradigm Shift from File System to DBMS
** **File System manages data using files on a hard disk. Users are allowed to create, delete, and update the files according to their requirements. Let us consider the example of file-based University Management System. Data of students is available to their respective Departments, Academics Section, Result Section, Accounts Section, Hostel Office, etc. Some of the data is common for all sections like Roll No, Name, Father Name, Address, and Phone number of students but some data is available to a particular section only like Hostel allotment number which is a part of the hostel office. Let us discuss the issues with this system:

- **Redundancy of data:** Data is said to be redundant if the same data is copied at many places. If a student wants to change their Phone number, he or she has to get it updated in various sections. Similarly, old records must be deleted from all sections representing that student.
- **Inconsistency of Data: **Data is said to be inconsistent if multiple copies of the same data do not match each other. If the Phone number is different in Accounts Section and Academics Section, it will be inconsistent. Inconsistency may be because of typing errors or not updating all copies of the same data.
- **Difficult Data Access:** A user should know the exact location of the file to access data, so the process is very cumbersome and tedious. If the user wants to search the student hostel allotment number of a student from 10000 unsorted students’ records, how difficult it can be.
- **Unauthorized Access:** File Systems may lead to unauthorized access to data. If a student gets access to a file having his marks, he can change it in an unauthorized way.
- **No Concurrent Access: **The access of the same data by multiple users at the same time is known as concurrency. The file system does not allow concurrency as data can be accessed by only one user at a time.
- **No Backup and Recovery:** The file system does not incorporate any backup and recovery of data if a file is lost or corrupted.
### Advantages of DBMS over File system: 
- **Data redundancy and inconsistency: **Redundancy is the concept of repetition of data i.e. each data may have more than a single copy. The file system cannot control the redundancy of data as each user defines and maintains the needed files for a specific application to run. There may be a possibility that two users are maintaining the data of the same file for different applications. Hence changes made by one user do not reflect in files used by second users, which leads to inconsistency of data. Whereas DBMS controls redundancy by maintaining a single repository of data that is defined once and is accessed by many users. As there is no or less redundancy, data remains consistent.
- **Data sharing: **The file system does not allow sharing of data or sharing is too complex. Whereas in DBMS, data can be shared easily due to a centralized system.
- **Data concurrency: **Concurrent access to data means more than one user is accessing the same data at the same time. Anomalies occur when changes made by one user get lost because of changes made by another user. The file system does not provide any procedure to stop anomalies. Whereas DBMS provides a locking system to stop anomalies to occur.
- **Data searching: **For every search operation performed on the file system, a different application program has to be written. While DBMS provides inbuilt searching operations. The user only has to write a small query to retrieve data from the database.
- **Data integrity: **There may be cases when some constraints need to be applied to the data before inserting it into the database. The file system does not provide any procedure to check these constraints automatically. Whereas DBMS maintains data integrity by enforcing user-defined constraints on data by itself.
- **System crashing: **In some cases, systems might have crashed due to various reasons. It is a bane in the case of file systems because once the system crashes, there will be no recovery of the data that’s been lost. A DBMS will have the recovery manager which retrieves the data making it another advantage over file systems. 
- **Data security: **A file system provides a password mechanism to protect the database but how long can the password be protected? No one can guarantee that. This doesn’t happen in the case of DBMS. DBMS has specialized features that help provide shielding to its data. 
- **Backup: **It creates a backup subsystem to restore the data if required.
- **Interfaces**: It provides different multiple user interfaces like graphical user interface and application program interface.
- **Easy Maintenance**: It is easily maintainable due to its centralized nature.
DBMS is continuously evolving from time to time. It is a powerful tool for data storage and protection. In the coming years, we will get to witness an AI-based DBMS to retrieve databases of ancient eras. 

![Figure 5](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---YoImnS5MLWXgVmgrYKHAw---figure---sQOnrldEsBj_WwpRFQhQDQ.png "Figure 5")

## Disadvantages of DBMS
- **Complexity:** DBMS can be complex to set up and maintain, requiring specialized knowledge and skills.
- **Performance overhead: **The use of a DBMS can add overhead to the performance of an application, especially in cases where high levels of concurrency are required.
- **Scalability: **The use of a DBMS can limit the scalability of an application, since it requires the use of locking and other synchronization mechanisms to ensure data consistency.
- **Cost:** The cost of purchasing, maintaining and upgrading a DBMS can be high, especially for large or complex systems.
- **Limited Use Cases:** Not all use cases are suitable for a DBMS, some solutions don’t need high reliability, consistency or security and may be better served by other types of data storage.
## Applications of DBMS
![Figure 6](/.eraser/SoAZWqIyNfuLnfJG69BC___v9mbn5vT6UcEXRnIU8fiBfvMxrF3___---figure---sntfR4ZTMiW1P9yLjat_c---figure---NUaedD517LSrhEbfAs6v_A.png "Figure 6")

- **Enterprise Information: **Sales, accounting, human resources, Manufacturing, online retailers.
- **Banking and Finance Sector: **Banks maintaining the customer details, accounts, loans, banking transactions, credit card transactions. Finance: Storing the information about sales and holdings, purchasing of financial stocks and bonds.
- **University: **Maintaining the information about student course enrolled information, student grades, staff roles.
- **Airlines: **Reservations and schedules.
- **Telecommunications: **Prepaid, postpaid bills maintenance.
## Conclusion
A Database Management System (DBMS) is an essential tool for efficiently managing, organizing, and retrieving large volumes of data across various industries. Its ability to handle data securely, ensure integrity, support concurrent access, and provide backup and recovery options makes it indispensable for modern data-driven applications. While DBMSs come with complexities and costs, their benefits in terms of data management and security far outweigh the challenges, making them a crucial component in any data-centric environment



<!--- Eraser file: https://app.eraser.io/workspace/SoAZWqIyNfuLnfJG69BC --->