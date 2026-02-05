# SQL

## Introduction
SQL stands for Structured Query Language. It is used to work with data stored in databases. Using SQL, we can insert new data, read existing data, update records, and delete unwanted data. SQL is commonly used in web applications, business reports, and data analysis systems because it makes handling large data easy.

## SQL Basics
SQL works with tables. A table contains rows and columns, where each row represents a record and each column represents a field.

### Common SQL Commands
- SELECT is used to read data from a table
- INSERT is used to add new records
- UPDATE is used to change existing records
- DELETE is used to remove records

### Example
SELECT name, age  
FROM students  
WHERE age > 18;

This query selects the name and age of students who are older than 18 years.

## SQL Joins
Joins are used when data is stored in multiple tables. They help combine related data using a common column.

### Types of Joins
- INNER JOIN returns only matching records from both tables
- LEFT JOIN returns all records from the left table
- RIGHT JOIN returns all records from the right table
- FULL JOIN returns all records from both tables

### Example
SELECT students.name, courses.course_name  
FROM students  
INNER JOIN courses  
ON students.course_id = courses.id;

This query displays student names along with their course names by joining two tables.

## SQL Aggregations
Aggregation functions are used to perform calculations on a group of rows and return a single result.

### Common Aggregation Functions
- COUNT returns the number of rows
- SUM returns the total value
- AVG returns the average value
- MIN returns the smallest value
- MAX returns the largest value

### Example
SELECT department, COUNT(*) AS total_employees  
FROM employees  
GROUP BY department;

This query shows how many employees are present in each department.

## Conclusion
SQL is an important tool for managing and analyzing data. Knowing SQL basics, joins, and aggregation functions helps in writing better queries and generating useful reports. These concepts are widely used in real-world applications and databases.

## References
- https://www.w3schools.com/sql/
- https://www.geeksforgeeks.org/sql-tutorial/
- https://www.mysqltutorial.org/
