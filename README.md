

# Elevate Labs - SQL Developer Internship Task 4

## Task Overview
This project is the fourth task for the SQL Developer Internship. [cite_start]The objective is to practice using aggregate functions and grouping to summarize and analyze data. [cite: 49]

- [cite_start]**Tools Used:** MySQL Workbench [cite: 50]

---
## SQL Queries
The `aggregate_queries.sql` file is the main deliverable for this task. It includes a series of queries that answer common business questions by summarizing data. The queries demonstrate the use of the following functions and clauses:
- [cite_start]`COUNT`, `SUM`, and `AVG` [cite: 51]
- [cite_start]`GROUP BY` to categorize data [cite: 54]
- [cite_start]`HAVING` to filter summarized groups [cite: 55]
- `ORDER BY` to sort the aggregated results.

---
## Interview Questions & Answers

### 1. What is GROUP BY?
[cite_start]The `GROUP BY` clause is used to arrange identical data into groups. [cite: 54] It's often used with aggregate functions (`COUNT`, `SUM`, `AVG`, etc.) to get a summary for each of those groups.

### 2. Difference between WHERE and HAVING?
The `WHERE` clause filters individual rows **before** any grouping or aggregation happens. [cite_start]The `HAVING` clause filters entire groups **after** the `GROUP BY` and aggregate functions have been applied. [cite: 55]

### 3. How does COUNT(*) differ from COUNT(column)?
[cite_start]`COUNT(*)` counts all rows in the result set. [cite: 61] [cite_start]`COUNT(column)` counts only the rows where the specified `column` is not `NULL`. [cite: 61]

### 4. Can you group by multiple columns?
[cite_start]Yes, you can. [cite: 62] When you `GROUP BY` multiple columns, the database creates groups based on the unique combination of values in those columns.

### 5. What is ROUND() used for?
[cite_start]The `ROUND()` function is used to round a numeric value to a specified number of decimal places, making the output cleaner and more readable. [cite: 63]

### 6. How do you find the highest salary by department?
[cite_start]You would use the `MAX()` aggregate function on the salary column and `GROUP BY` the department column. [cite: 64] The query would look like: `SELECT department, MAX(salary) FROM employees GROUP BY department;`.

### 7. What is the default behavior of GROUP BY?
[cite_start]The default behavior of `GROUP BY` is to collect all rows with the same value in the specified column(s) into a single summary row. [cite: 65]

### 8. Explain AVG and SUM.
[cite_start]`AVG` is an aggregate function that calculates the average value of a numeric column. [cite: 51, 66] [cite_start]`SUM` is an aggregate function that calculates the total sum of a numeric column. [cite: 51, 66]

### 9. How to count distinct values?
[cite_start]You count distinct (unique) values by using the `DISTINCT` keyword inside the `COUNT` function, like this: `COUNT(DISTINCT column_name)`. [cite: 67]

### 10. What is an aggregate function?
[cite_start]An aggregate function performs a calculation on a set of values (like a column) and returns a single, summary value. [cite: 53, 68] Common examples include `COUNT`, `SUM`, `AVG`, `MAX`, and `MIN`.
