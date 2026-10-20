Data Transformer
Overview
This project demonstrates SQL data transformation and analysis using a sample database named Data_Transformer.

It creates three tables:
- Customers — customer details and registration dates.
- Orders — order details, customer references, dates, and total amounts.
- Employees — employee details, departments, hire dates, and salaries.
Features
- Creates the database and tables with primary and foreign key constraints.
- Inserts sample data into the tables.
- Demonstrates INNER JOIN, LEFT JOIN, and RIGHT JOIN.
- Demonstrates a FULL OUTER JOIN equivalent using LEFT JOIN, RIGHT JOIN, and UNION ALL (since MySQL does not directly support FULL OUTER JOIN).
- Finds orders above the average order amount.
- Finds employees earning above the average salary.
- Extracts year and month from order dates.
- Calculates days since each order and formats order dates.
- Uses string functions such as CONCAT, REPLACE, UPPER, LOWER, and TRIM.
- Calculates a running total and ranks orders by amount.
- Uses CASE expressions to calculate order discounts and categorize employee salaries.
Database Tables
Table	Purpose
Customers	Stores customer ID, name, email, and registration date.
Orders	Stores order ID, customer ID, order date, and total amount.
Employees	Stores employee ID, name, department, hire date, and salary.


Requirements
- MySQL 8.0+ is recommended for window functions such as SUM() OVER and RANK() OVER.
- A SQL client that can run MySQL scripts.
How to Run
1. Open your MySQL client.
2. Open DATA_TRANSFORMER (1).sql.
3. Execute the script.
4. Run or review the SELECT queries to see the results.
Notes
- The script drops the Orders, Customers, and Employees tables if they already exist before recreating them.
- The sample data is inserted each time the script is run.
- The discount rules are: orders above 1000 receive 10%, orders above 500 receive 5%, and all others receive 0%.
- Salary categories are based on the assumptions in the SQL script: High for salaries of 70000 or more, Medium for salaries of 50000 or more but below 70000, and Low for salaries below 50000.
