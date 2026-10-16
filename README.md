# Data Transformer – SQL Project

## 📌 Project Overview

The **Data Transformer** project is designed to practice and demonstrate SQL skills using MySQL. This project focuses on database creation, data management, joins, subqueries, date functions, string functions, window functions, and conditional statements.

It helps understand how SQL can be used to retrieve, transform, and analyze data efficiently.

## 🎯 Project Objectives

- Create and manage a database using MySQL.
- Store customer, order, and employee information.
- Understand and implement different types of SQL joins.
- Use subqueries to analyze data.
- Apply date and string functions.
- Calculate running totals and rankings.
- Use CASE statements for conditional data analysis.

## 🛠️ Technologies Used

- **Database:** MySQL
- **Language:** SQL
- **Tool:** MySQL Workbench (or any compatible MySQL client)

## 🗄️ Database Structure

The project uses a database named `data_transformer` with three tables.

### 1. Customers

Stores customer information.

| Column | Description |
|---|---|
| CustomerID | Unique customer identifier (Primary Key) |
| Firstname | Customer's first name |
| Lastname | Customer's last name |
| Email | Customer's email address |
| RegistrationDate | Customer registration date |

### 2. Orders

Stores order details and connects orders to customers.

| Column | Description |
|---|---|
| OrderID | Unique order identifier (Primary Key) |
| CustomerID | Customer reference (Foreign Key) |
| OrderDate | Date of the order |
| TotalAmount | Total order amount |

### 3. Employees

Stores employee information.

| Column | Description |
|---|---|
| EmployeeID | Unique employee identifier (Primary Key) |
| Firstname | Employee's first name |
| Lastname | Employee's last name |
| Department | Employee's department |
| HireDate | Employee hiring date |
| Salary | Employee salary |

## 📚 SQL Concepts Covered

### 1. Joins
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- FULL OUTER JOIN logic using LEFT JOIN, RIGHT JOIN, and UNION in MySQL

### 2. Subqueries
- Find orders with amounts above the average order amount.
- Find employees earning above the average salary.

### 3. Date Functions
- YEAR()
- MONTH()
- DATEDIFF()
- DATE_FORMAT()
- CURRENT_DATE()

### 4. String Functions
- CONCAT()
- REPLACE()
- UPPER()
- LOWER()
- TRIM()

### 5. Window Functions
- SUM() OVER() for running totals
- RANK() OVER() for ranking orders by amount

### 6. Conditional Statements
- CASE WHEN for discount calculation
- CASE WHEN for employee salary categorization

## 💡 Key Learning Outcomes

- Understanding primary and foreign keys.
- Joining related tables using common identifiers.
- Analyzing data using aggregate functions and subqueries.
- Formatting and transforming text and date values.
- Applying window functions for analytical calculations.
- Categorizing data using conditional logic.

## ▶️ How to Run the Project

1. Install MySQL Server and MySQL Workbench.
2. Open MySQL Workbench and connect to your database server.
3. Create the database and tables using the SQL script.
4. Insert the sample data into all three tables.
5. Execute the SQL queries one by one.
6. Review the output of each query to understand the results.

**Important:** Execute the table creation and INSERT statements before running the analysis queries. Ensure the JOIN conditions correctly match `Customers.CustomerID` with `Orders.CustomerID`.

## 📂 Project File Structure

```text
Data-Transformer/
│
├── README.md
└── data_transformer.sql
```

## 👨‍💻 Author

Created as a SQL learning project to practice database management and data analysis concepts.

## 📄 License

This project is intended for educational and learning purposes.
