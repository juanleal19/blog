---
layout: post
title: Getting Started with PostgreSQL
---

# Installation of PostgreSQL

To begin your journey with PostgreSQL, the first step is to install it on your system. Follow these installation steps:

1. Download and install [PostgreSQL](https://www.postgresql.org/download/) from the official website.

2. During the installation, make sure to remember the password you set. You'll need it later.

## Getting Started with PostgreSQL

Now that you have PostgreSQL installed, let's start working with it using the SQL Shell.

### Creating a Database

To create a new database, open the SQL Shell and execute the following command:

```SQL
CREATE DATABASE database_name;
```
if it woors you shoul se a mesage "CREATE DATABASE"
### Errasing a Database
To errase a database, open pgAdmin and log in to Servers(), use the passwor and try to errase the database. 
![Image of reference pgAdmin V4 16.0.1](C:\Users\jujuj\OneDrive\Escritorio\blog\images\404.jpg``)

# SQL Basics

Before we dive into using PostgreSQL, let's cover some fundamental SQL commands. These commands will help you understand the basics of querying a database.

## SELECT Statement

The `SELECT` statement is one of the most fundamental commands in SQL. It is used to retrieve data from one or more tables. Here are a few examples to illustrate its usage:

1. **Retrieve all columns from `Table_1`:**

```
ELECT *
FROM Table_1 AS t1
JOIN Table_2 AS t2
ON t1.primary_key = t2.foreign_key;
```
In this case, we are selecting data from both **Table_1** (aliased as **t1**) and **Table_2** (aliased as **t2**). We are performing a join operation based on the equality of the **primary_key** in **t1** and the **foreign_key** in **t2**. This allows us to combine data from both tables based on the specified relationship.

more about [`Primery key & foreign_ket`](https://juanleal19.github.io/blog/Hello-World/)

Let's explore some additional examples of the SELECT statement:

1. **Select Specific Columns**
   You can select specific columns by listing them instead of using the asterisk. For instance, to retrieve only the `column1` and `column2` from `Table_1`:
   ``` s
    SELECT column1, column2
    FROM Table_1;
   ```
2. **Filter Rows with the WHERE Clause**
   To filter rows based on a specific condition, use the `WHERE` clause. For example, retrieve rows from `Table_1` where the `column3` is equal to `'value'`:
   ```
   SELECT *
   WHERE column3 = 'value';
   ```
3. ***Aggregate Functions***
   SQL allows you to perform aggregate functions like `SUM`, `COUNT`, `AVG`, etc. Here's an example of calculating the total sales amount from a sales table:
   ```
   SELECT SUM(sales_amount) AS total_sales
   FROM SalesTable;
   ```
   SELECT SUM(sales_amount) AS total_sales
   FROM SalesTable;

