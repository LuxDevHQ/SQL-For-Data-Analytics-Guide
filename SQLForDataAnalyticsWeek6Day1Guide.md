## **Lesson Plan.**

#### Day 1: Introduction to SQL & Data Retrieval

**Duration:** 3 hours  

##### Topics Covered  

- **Introduction to Databases & SQL**  
  - What is SQL?  
  - Importance of SQL in Data Analytics  
  - Relational Databases & SQL vs NoSQL  

- **Basic SQL Commands**  
  - `SELECT`, `FROM`, `WHERE`  
  - Filtering using comparison (`=, <, >, <=, >=, <>`) & logical operators (`AND`, `OR`, `NOT`)  
  - Using `DISTINCT`  

- **Sorting and Limiting Results**  
  - `ORDER BY` (Ascending & Descending)  
  - `LIMIT`  

- **Basic Aggregations**  
  - `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`  
  - `GROUP BY` & `HAVING`  

##### Practice Assignments  

- Retrieve data based on conditions (e.g., employees earning above a certain salary).  
- Use `GROUP BY` to find average sales per product.

## **Lesson Content.**
### Day 1: Introduction to SQL & Data Retrieval  
**Duration:** 3 hours  

## **Lesson Plan**

### **Hour 1: Introduction to Databases & SQL**

#### **What is SQL?**
- SQL stands for Structured Query Language.
- It is used to interact with relational databases.
- SQL allows you to create, read, update, and delete data (CRUD operations).

#### **Why is SQL Important for Data Analytics?**
- SQL helps in data extraction from large datasets efficiently.
- It allows analysts to filter, aggregate, and transform data before visualization.
- SQL is widely used in Business Intelligence and Data Science fields.

#### **Understanding Relational Databases**
- Data is stored in tables (rows & columns).
- Tables are related using **Primary Keys** and **Foreign Keys**.
- Examples of relational databases: MySQL, PostgreSQL, SQL Server, SQLite.

#### **Basic SQL Commands Overview**
- `SELECT` - Retrieves data from tables.
- `FROM` - Specifies the table to retrieve data from.
- `WHERE` - Filters data based on conditions.

### **Hour 2: Writing SQL Queries**

#### **Retrieving Data from a Table**
```sql
SELECT * FROM employees;
```
- Retrieves all columns from the `employees` table.

#### **Filtering Data with WHERE Clause**
```sql
SELECT * FROM employees WHERE salary > 50000;
```
- Returns employees with salaries above 50,000.

#### **Using Logical Operators**
```sql
SELECT * FROM employees WHERE department = 'Sales' AND salary > 40000;
```
- Fetches employees in Sales with salaries above 40,000.

#### **Sorting Data Using ORDER BY**
```sql
SELECT name, salary FROM employees ORDER BY salary DESC;
```
- Orders employees by salary in descending order.

#### **Limiting Results Using LIMIT**
```sql
SELECT * FROM employees LIMIT 5;
```
- Returns only the first 5 records.

### **Hour 3: Aggregations & Grouping Data**

#### **Basic Aggregation Functions**
- `COUNT()` - Counts the number of rows.
- `SUM()` - Calculates the total sum of a column.
- `AVG()` - Computes the average value.
- `MIN()` / `MAX()` - Finds the smallest/largest value.

#### **Examples:**
```sql
SELECT COUNT(*) FROM employees;
```
- Returns the total number of employees.

```sql
SELECT AVG(salary) FROM employees;
```
- Computes the average salary of employees.

```sql
SELECT department, SUM(salary) FROM employees GROUP BY department;
```
- Groups employees by department and calculates total salary for each.

#### **Filtering Grouped Data with HAVING**
```sql
SELECT department, AVG(salary) FROM employees GROUP BY department HAVING AVG(salary) > 60000;
```
- Returns departments with an average salary above 60,000.

### **Practice Assignments**
- Retrieve employees earning above a certain salary.
- Sort employees based on different attributes.
- Use `GROUP BY` to analyze sales per product.

---
This structured lesson will ensure freshers grasp SQL fundamentals efficiently in a 3-hour session. 🚀


  

