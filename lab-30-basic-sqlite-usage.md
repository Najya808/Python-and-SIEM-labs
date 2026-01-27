 Lab 30: Basic SQLite Usage

 What I Learned
In this lab, I learned how to use SQLite with Python using the built-in `sqlite3` module. I practiced creating an in-memory database, defining tables, inserting records, querying data, and fetching results. This lab introduced me to basic database operations that are essential for data storage and retrieval in real-world applications.

---

 Objectives
- Understand how to use SQLite in Python
- Establish a connection to an SQLite database
- Create tables and insert data
- Query tables and fetch results
- Print and interpret database records

---

 Prerequisites
- Basic understanding of Python programming
- Python installed on the system
- A code editor or IDE (VSCode, PyCharm, or terminal)

---

 Lab Tasks Performed

 Task 1: Importing the SQLite Module

```python
import sqlite3
Explanation:
The sqlite3 module is included in Python’s standard library, so no additional installation is required.

Task 2: Connecting to an SQLite Database
python
Copy code
connection = sqlite3.connect(':memory:')
Explanation:
An in-memory database is created, which exists only while the program is running. This is useful for testing and temporary data storage.

Task 3: Creating a Table
python
Copy code
cursor = connection.cursor()

cursor.execute("""
CREATE TABLE students (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    grade REAL
)
""")
Key Concept – Cursor:
A cursor allows execution of SQL commands and retrieval of query results from the database.

Task 4: Inserting Data into the Table
python
Copy code
students_data = [
    (1, 'Alice', 85.5),
    (2, 'Bob', 78.0),
    (3, 'Charlie', 92.0)
]

cursor.executemany("INSERT INTO students VALUES (?, ?, ?)", students_data)
connection.commit()
Explanation:

executemany() efficiently inserts multiple rows

Parameterized queries (?) protect against SQL injection

commit() saves the changes to the database

Task 5: Querying the Table
python
Copy code
cursor.execute("SELECT * FROM students")
results = cursor.fetchall()
Key Concept – SQL Query:
SQL is used to retrieve structured data from the database using commands like SELECT.

Task 6: Fetching and Printing Results
python
Copy code
for row in results:
    print(row)
Explanation:
Each row from the database is printed, allowing verification of stored data.

 Sample Output
bash
Copy code
(1, 'Alice', 85.5)
(2, 'Bob', 78.0)
(3, 'Charlie', 92.0)

 Summary
This lab demonstrated the core steps involved in using SQLite with Python:

Connecting to a database

Creating tables

Inserting records

Querying and displaying data

These foundational skills are essential for building applications that require persistent data storage.
