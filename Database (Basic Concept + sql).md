# DataBase Basics

### What is a Database?
Answer: A database is a structured collection of data organized in a way that a computer program can quickly select and retrieve specific pieces of data.


### What is dbms?
DBMS stands for Database Management System. It is software that enables users to interact with databases, providing functionalities for data storage, retrieval, update, and management.

### Relational Database?
Relational database: A relational database is the most common type of database. It organizes data into tables, each consisting of rows and columns. Primary and foreign keys define the relationships between tables.

### Explain the difference between a DBMS and a RDBMS.
Answer: A DBMS (Database Management System) manages data in a general way, while an RDBMS (Relational Database Management System) specifically manages data using a relational model, involving tables with rows and columns, and enforcing relationships between tables.    
1. **DBMS Supports data storage in various formats.  RDBMS Organizes data in a tabular format with rows and columns.**    
2. **DBMS Enforces relationships between tables using primary and foreign keys.   RDBMS May not enforce relationships between tables.**

### What is denormalization?
Answer: Denormalization is the process of introducing redundancy into a database by combining tables or adding redundant data. It is done to improve query performance by reducing the need for complex joins.

### what is sql?
Structured Query Language (SQL) is a programming language used to manage and manipulate data in a relational database. SQL allows you to perform a wide range of operations, including querying, inserting, updating, and deleting data.

### Difference between sql and mysql
![image](https://github.com/Abdul-Aziz026/DataBase-interview-Question/assets/57495952/b7f51dda-60ec-40f1-8d97-5e636cc8aac0)

### what is data mining?
Data mining is the process of discovering patterns and insights from large datasets. It is often used in business and scientific research to identify trends and make predictions.

### What is a primary key?
Answer: A primary key is a unique identifier for a record in a table. It must be unique for each record, and it cannot contain null values. Primary keys are used to establish relationships between tables.

### What is a foreign key?
Answer: A foreign key is a column or a set of columns in a table that refers to the primary key of another table. It establishes a link between the two tables, enforcing referential integrity.

### Explain the difference between INNER JOIN and LEFT JOIN.
Answer: INNER JOIN returns only the matching rows from both tables, while LEFT JOIN returns all the rows from the left table and the matching rows from the right table. If there is no match, the result will contain NULL values for columns from the right table.


### difference between int and bigint in sql?
<ins>**INT:**</ins> Typically, INT occupies 4 bytes (32 bits) of storage. int range is -2,147,483,648 to 2,147,483,647.   
<ins>**BIGINT:**</ins> its use 8 bytes (64 bits) of storage.Bigint is like c++ long long it ranges from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.

### What is normalization and denormalization?
Normalization      V/S       	Denormalization   
1. <ins>**Goal:**</ins>	Normalization Reduce redundancy and dependency.	  
Denormalization Improve query performance.  
2. <ins>**Process:**</ins>	Normalization Organize data into smaller, related tables.	  
Denormalization Introduce some redundancy to reduce joins.   
3. <ins>**Advantages:**</ins>	Normalization Minimize data redundancy, ensure consistency.   
Denormalization Faster query performance, simpler queries.    
4. <ins>**Disadvantages:**</ins>	Normalization May lead to more tables, complex queries.	   
Denormalization Increases data redundancy, maintenance complexity.

### what is self join?
A self join in SQL is a specific type of join where a table is joined with itself.

### what is data redundancy?
Data redundancy occurs when the same piece of data exists in multiple places, whereas data inconsistency is when the same data exists in different formats in multiple tables.

### what is data inconsistency?
there are more than 2 tables within a database that work with the same data but receive it from different inputs.aikhane 2 ta table a salary ar name ache. to 2 table a akoi name er salary different atakei data inconsistency bole.

### data atomicity?.
Atomicity is a property of database transactions that ensures that a set of database operations either all occur, or none occur. (aikhane kokhono data ordhek upload hobe ar ordehek hobe na erokom kokhono hobe na. hole sobgulo upload hobe otherwise aktao hobe na)

### what is candidate key?
The minimal set of attributes that can be uniquely identify a tuple is known as a candidate key. A candidate key is a subset of a super key set where the key which contains no redundant attribute is none other than a Candidate Key.candidate key null hote parbe. jemon akjon student er email candidate key.so email nao thakte pare. aikhane email er jaygae null hobe.

### what is super key?
super key is a single key or a group of multiple keys that can uniqly identify tuples in a table.
