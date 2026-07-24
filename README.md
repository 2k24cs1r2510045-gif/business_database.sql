# Business Management Database using MySQL

## 📌 Project Description

This project is a simple Business Management Database developed using MySQL. It demonstrates database creation, table creation, inserting records, and retrieving data using SQL queries.

---

## 📂 Database Name

BusinessDB

---

## Tables

### Customers
Stores customer information.

| Column | Data Type |
|---------|-----------|
| CustomerID | INT |
| CustomerName | VARCHAR(100) |
| Email | VARCHAR(100) |
| Phone | VARCHAR(15) |
| City | VARCHAR(50) |

---

### Products

Stores product information.

| Column | Data Type |
|---------|-----------|
| ProductID | INT |
| ProductName | VARCHAR(100) |
| Category | VARCHAR(50) |
| Price | DECIMAL(10,2) |
| Stock | INT |

---

### Orders

Stores customer orders.

| Column | Data Type |
|---------|-----------|
| OrderID | INT |
| CustomerID | INT |
| ProductID | INT |
| Quantity | INT |
| OrderDate | DATE |

---

## Features

- Create Database
- Create Tables
- Primary Keys
- Foreign Keys
- Insert Records
- SELECT Queries
- JOIN Queries

---

## Technologies Used

- MySQL
- SQL
- MySQL Workbench

---

## Sample Query

```sql
SELECT
c.CustomerName,
p.ProductName,
o.Quantity,
o.OrderDate
FROM Orders o
JOIN Customers c
ON o.CustomerID = c.CustomerID
JOIN Products p
ON o.ProductID = p.ProductID;
```

---

## Author

**Priyanshi Sharma**

B.Tech CSE Student

PSIT Kanpur

---
