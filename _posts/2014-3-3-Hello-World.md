---
layout: post
title: PK & FK
---

# Primary Key

A **primary** key is a column or a set of columns in a database table that uniquely identifies each row or record in that table. Here are some key points about primary keys:

1. Uniqueness: Every value in the primary key column(s) must be unique within the table. This ensures that no two rows in the table can have the same primary key value.

2. Non-null: The values in the primary key column(s) cannot be NULL (i.e., empty or missing). This guarantees that each row has a valid identifier.

3. Indexing: Primary keys are often indexed by the database management system for fast retrieval and to enforce uniqueness.

4. Relationships: Primary keys are commonly used to establish relationships between tables. Other tables can reference the primary key of a table as a foreign key to create associations between data.

5. Example: In a database of employees, an "EmployeeID" column could be used as the primary key to uniquely identify each employee record. This ensures that no two employees have the same EmployeeID.

# Foreign Key
A **foreign** key is a column or a set of columns in one table that is used to establish a link or relationship with the primary key of another table. Foreign keys are used to maintain referential integrity within a relational database. Here are some key points about foreign keys:

1. Referential Integrity: Foreign keys enforce referential integrity by ensuring that values in the foreign key column(s) of one table correspond to the values in the primary key column(s) of another table. This maintains the consistency and validity of data across related tables.

2. Relationships: Foreign keys define relationships between tables. They indicate that there is a connection between data in one table and data in another.

3. Cascading Actions: Foreign keys can be configured to perform cascading actions when changes are made to the referenced primary key. For example, you can set up cascading deletes to automatically delete related records when a primary key is deleted.

4. Example: In a database that includes an "Orders" table and a "Customers" table, the "CustomerID" column in the "Orders" table can be a foreign key that references the "CustomerID" primary key in the "Customers" table. This establishes a relationship between customer records and their corresponding orders.