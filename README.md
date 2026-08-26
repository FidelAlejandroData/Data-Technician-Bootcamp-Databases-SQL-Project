# SQL Database & Data Analysis Project – Data Technician Bootcamp

In this repository, I showcase the database exercises, SQL queries and supporting materials I completed during the **Week 3 Databases & SQL module of the Data Technician Bootcamp**.

## 📊 Project Overview

During this project, I developed an understanding of **relational databases** and used SQL to retrieve, filter, combine and analyse structured data.

I combined database theory with practical exercises using **PostgreSQL and Supabase**, including work with retail-style data involving customers, products, sales, inventory, suppliers and loyalty information.

## 🔄 My SQL Analysis Workflow

```mermaid
flowchart LR
    A[🗄️ Database] --> B[🔎 SELECT]
    B --> C[🎯 WHERE]
    C --> D[↕️ ORDER BY]
    D --> E[📊 GROUP BY]
    E --> F[🔗 JOIN]
    F --> G[🧮 Aggregate]
    G --> H[💡 Extract Insights]
```

## 🛠️ Skills I Demonstrated

### 💻 Core SQL Queries

I practised using:

* `SELECT`
* `FROM`
* `WHERE`
* `ORDER BY`
* `GROUP BY`
* `HAVING`
* `DISTINCT`

### 🧮 Aggregate Functions

I used:

* `COUNT()`
* `SUM()`
* `AVG()`
* `MIN()`
* `MAX()`

to summarise information and calculate useful metrics.

### 🔗 SQL JOINs

I explored different ways of combining tables using:

* `INNER JOIN`
* `LEFT JOIN`
* `RIGHT JOIN`
* `FULL JOIN`
* `CROSS JOIN`
* `SELF JOIN`

### 🔎 Filtering & Conditions

I worked with:

* `AND`
* `OR`
* `NOT`
* `IN`
* `BETWEEN`
* `LIKE`

to create more specific queries.

### 🗃️ Database Design

I developed an understanding of:

* Tables
* Primary keys
* Foreign keys
* Relationships
* One-to-one relationships
* One-to-many relationships
* Many-to-many relationships
* Entity Relationship Diagrams and Schemas

## 📈 Key Project Activities

### 🛍️ Retail Database Design

I designed a relational database structure capable of managing:

* 📅 Dates
* 👤 Customers
* 📦 Products
* 🧾 Sales
* 💰 Costs
* 🎟️ Loyalty information
* 🏪 Inventory
* 🚚 Suppliers

### 🔗 Database Relationships Example

```mermaid
erDiagram
    CUSTOMER ||--o{ SALES : makes
    PRODUCT ||--o{ SALES : appears_in
    SUPPLIER ||--o{ PRODUCT : supplies
    PRODUCT ||--|| INVENTORY : has

    CUSTOMER {
        int customer_id
        string name
    }

    SALES {
        int transaction_id
        int customer_id
        int product_id
        int quantity
    }

    PRODUCT {
        int product_id
        string product_name
        decimal price
    }

    SUPPLIER {
        int supplier_id
        string supplier_name
    }

    INVENTORY {
        int product_id
        int stock_quantity
    }
```

This helped me understand how primary and foreign keys are used to connect information across different tables. The following diagram illustrates the galaxy schema I created:

<img width="640" height="741" alt="image" src="https://github.com/user-attachments/assets/6d6ac0c5-88d6-4cdb-b370-7dd8b6522677" />

### 💻 SQL Query Practice

Using PostgreSQL through **Supabase**, I wrote queries to:

* Retrieve specific records
* Filter information
* Sort results
* Group data
* Calculate totals and averages
* Combine information from different tables

### 🧩 JOIN Analysis

I used JOINs to understand how separate datasets can be combined to answer questions such as:

* Which customers purchased each product?
* Which products generate the most sales?
* Which suppliers provide specific products?
* Which categories perform best?

### 🛠️ Query Debugging

I also identified and corrected syntax errors in SQL queries.

This helped strengthen my understanding of SQL structure and improved my problem-solving skills.

## 💡 Data Analysis with SQL

I learned to use SQL not simply to retrieve records, but to transform database information into analytical outputs.

```mermaid
flowchart TD
    A[🧾 Raw Transactions] --> B[🔎 Filter]
    B --> C[📊 Group]
    C --> D[🧮 Aggregate]
    D --> E[🔗 Add Context with JOINs]
    E --> F[💡 Business Insight]
```

## 🎯 Learning Outcomes

By completing this project, I developed practical experience in:

* SQL query writing
* PostgreSQL
* Supabase
* Relational databases
* Database design
* Primary and foreign keys
* Filtering
* Sorting
* Grouping
* Aggregation
* SQL JOINs
* Subqueries
* ERDs
* Query debugging
* Extracting insights from structured data

## 🏅 Related Certifications

To complement the practical SQL work completed in this project, I also completed:

* 🎓 [**Introduction to SQL – DataCamp**](https://www.datacamp.com/completed/statement-of-accomplishment/course/b57798930b3041fb50e37266716d97f3961bee33?utm_medium=organic_social&utm_campaign=sharewidget&utm_content=soa)
* 🎓 [**Intermediate SQL – DataCamp**](https://www.datacamp.com/completed/statement-of-accomplishment/course/99ce9a4f22474d933eba1981d06faca60d186335?utm_medium=organic_social&utm_campaign=sharewidget&utm_content=soa)
* 🎓 [**Joining Data in SQL – DataCamp**](https://www.datacamp.com/completed/statement-of-accomplishment/course/b975050579e347545d313a33f7894f7e6e8503e9?utm_medium=organic_social&utm_campaign=sharewidget&utm_content=soa)
* 🎓 [**Data Manipulation in SQL – DataCamp**](https://www.datacamp.com/completed/statement-of-accomplishment/course/bdcaed25416c3b95feb1ac0dee32adeb2efef920?utm_medium=organic_social&utm_campaign=sharewidget&utm_content=soa)

## 💻 Tools I Used

`SQL` `PostgreSQL` `Supabase` `Relational Databases` `ERD` `SQL JOINs` `Data Analysis`

## 📁 Project Contents

```text
📦 SQL-Database-Project
┣ 🗄️ Database exercises
┣ 💻 SQL queries
┣ 🧩 ERD / database diagram example
┣ 📊 Databases and SQL workbook
┣ 🧮 Supporting tables
┣ 🗃️ SQL Database Schema
┣ 📁 certificates
┃ ┣ 📄 DataCamp Certificate - Introduction to SQL.pdf
┃ ┣ 📄 DataCamp Certificate - Intermediate SQL.pdf
┃ ┣ 📄 DataCamp Certificate - Joining Data in SQL.pdf
┃ ┗ 📄 DataCamp Certificate - Data Manipulation in SQL.pdf
┗ 📄 README.md
```
