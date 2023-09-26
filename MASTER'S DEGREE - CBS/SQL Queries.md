SQL queries are commands used to communicate with and manipulate databases using the [[Structured Query Language (SQL)]].
### A Typical SQL Query:
![[Pasted image 20230926121626.png]]
A = represents an attribute
R = represents a relation
P = is a predicate

## The SELECT, FROM, and WHERE Clause
See [[SELECT, FROM, and WHERE Clause (SQL]]

## Common SQL Queries
1. **SELECT** - Retrieve data from one or more tables.
```SQL
SELECT column1, column2 FROM table_name WHERE condition;
```   

- Can rename “salary/12” using the as clause:  
```SQL
select ID, name, salary/12 as monthly_salary
```
   
2. **INSERT INTO** - Add new rows of data to a table.
```SQL
INSERT INTO table_name (column1, column2) VALUES (value1, value2);
```   

3. **UPDATE** - Modify existing data in a table.
```SQL
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```   

4. **DELETE** - Remove rows from a table.
```SQL
DELETE FROM table_name WHERE condition;
```   

5. **CREATE TABLE** - Create a new table.
```SQL
CREATE TABLE table_name (
   column1 datatype,
   column2 datatype,
   ...
);
```   

6. **ALTER TABLE** - Modify the structure of an existing table.
```SQL
ALTER TABLE table_name ADD COLUMN column_name datatype;
```   

7. **DROP TABLE** - Delete an existing table and all of its data.
```SQL
DROP TABLE table_name;
```   

8. **JOIN** - Combine rows from two or more tables based on a related column.
```SQL
SELECT column1, column2
FROM table1
INNER JOIN table2 ON table1.column = table2.column;
```   

#### For more info see [[Joins (SQL)]]

9. **GROUP BY** - Group rows that have the same values in specified columns into summary rows.
```SQL
SELECT column_name, COUNT(*)
FROM table_name
GROUP BY column_name;
```   

10. **ORDER BY** - Sort the result set in ascending or descending order.
```SQL
SELECT column1, column2 FROM table_name ORDER BY column1 ASC;
```   

11. **BETWEEN** - A comparison operator for saying between these two values
```SQL
select name from instructor where salary between 90000 and 100000
```

12. **UNION** - Will combine two queries into one (provided they have the same columns)
```SQL
(select course_id from section where sem = ‘Fall’ and year = 2009)
union 
(select course_id from section where sem = ‘Spring’ and year = 2010)
```

13. **INTERSECT** - Will find similar records between two sets
```SQL
(select course_id from section where sem = ‘Fall’ and year = 2009) 
intersect
(select course_id from section where sem = ‘Spring’ and year = 2010)
```


## String Operations in SQL
SQL includes a string-matching operator for comparisons on character strings. The operator like uses patterns that are described using two special characters:
- percent ( % ). - The % character matches any substring.
- underscore ( _ ). - The _ character matches any character.

Example, find the names of all instructors whose name includes the substring “dar”:
```SQL
select name from instructor where name like '%dar%
```

- Patterns are case sensitive.
- Pattern matching examples:
	- ``‘Intro%’`` matches any string beginning with “Intro”
	- ``‘%Comp%’`` matches any string containing “Comp” as a substring.
	- ``‘_ _ _’`` matches any string of exactly three characters.
	- ``‘_ _ _ %’`` matches any string of at least three characters.

- SQL supports a variety of string operations such as:
	- concatenation (using “||”)
	- converting from upper to lower case (and vice versa)
	- finding string length, extracting substrings, etc

### NULL Values in SQL
It is possible for tuples to have a null value, denoted by null, for some of their attributes
- The result of any arithmetic expression involving null is null 
	- Example: 5 + null returns null
- The predicate is null can be used to check for null values. 
	- Example: Find all instructors whose salary is null:
```SQL
select name from instructor where salary is null
```

### AGGREGATE Functions in SQL
These functions operate on the multiset of values of a column of a relation, and return a value
- ``avg``: average value 
- ``min``: minimum value 
- ``max``: maximum value 
- ``sum``: sum of values 
- ``count``: number of values

*Examples:*
Find the average salary of instructors in the Computer Science department
```SQL
select avg (salary) from instructor where dept_name= ’Comp. Sci.’;
```
Find the total number of instructors who teach a course in the Spring 2010 semester
```SQL
select count (distinct ID) from teaches where semester = ’Spring’ and year = 2010;
```
Find the number of tuples in the course relation
```SQL
select count (*) from course
```

- If you EVER use a function (e.g. sum(price)) and combine it with a column outside the function, you HAVE to use "Groupby"
E.g. 
```SQL
Select PID, SUM(Price)
From ProductSale
Group by PID
```

#### The HAVING Clause
The `HAVING` clause is used to filter the results of a SQL query based on aggregate functions. It is often used in conjunction with the `GROUP BY` clause to allow you to filter the grouped results.

Example, find the names and average salaries of all departments whose average salary is greater than 42000 
```SQL
select dept_name, avg (salary) from instructor group by dept_name having avg (salary) > 42000
```


### VIEWS in SQL
In PostgreSQL, a view is a virtual table based on the result-set of a SELECT statement. A view contains rows and columns, just like a real table, and it is stored in the database. However, the fields in a view are fields from one or more real tables in the database.

You can use views to:
- **Simplify Complex Queries**: If you have a complex query that you use frequently, you can save it as a view to avoid writing the query every time.
- **Enhance Security**: By creating views, you can restrict the degree of exposure of the underlying tables to the outer world.
- **Aggregate Data**: Views allow you to display aggregated and summarized data.
- **Join Tables**: You can create a view that joins columns from multiple tables, simplifying data retrieval.


In some cases, it is not desirable for all users to see the entire logical model (that is, all the actual relations stored in the database.
- A view provides a mechanism to hide certain data from the view of certain users.
- Any relation that is not of the conceptual model but is made visible to a user as a “virtual relation” is called a view.
- Views are widely used to provide access for Visual Dashboards

Example:
```SQL
CREATE VIEW high_salary_employees AS
SELECT first_name, last_name
FROM employees
WHERE salary > 50000;
```

So views are kinda like functions/methods in programming, where they can contain a query - everything after the AS will be run when we use the "high_salary_employees"