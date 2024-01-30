These clauses are utilised in the [[Structured Query Language (SQL)]] to interact with [[Databases]] and their [[Data]].


### General Structure 
```SQL
SELECT column1, column2 FROM table_name WHERE condition;
``` 

## SELECT Clause
The ``select`` clause is used to retrieve data from one or more tables.  

SQL allows duplicates in relations as well as in query results.  
- To force the elimination of duplicates, insert the keyword distinct after select.  
```SQL
select distinct dept_name from instructor
```

An asterisk in the select clause denotes “all attributes”  
```
select *  
from instructor  
```

An attribute can be a literal with no from clause  
```SQL
select ‘437’  
```
- Results is a table with one column and a single row with value “437” 

The select clause can contain arithmetic expressions involving the operation, +, –, \*, and /, and operating on  constants or attributes of tuples.  
- The query below would return a relation that is the same as the instructor relation, except that the value of the attribute salary  is divided by 12.  
```SQL
select ID, name, salary/12  
from instructor 
```

- Can rename “salary/12” using the as clause:  
```SQL
select ID, name, salary/12 as monthly_salary
```

## WHERE Clause
The ``where`` clause specifies conditions that the result must satisfy

E.g. to find all instructors in Comp. Sci. dept:
```SQL
select name 
from instructor 
where dept_name = 'Comp. Sci.'
```

- Comparison results can be combined using the logical connectives ``and``, ``or``, and ``not`` 
- To find all instructors in Comp. Sci. dept with salary > 80000:
```SQL
select name. from instructor where dept_name = 'Comp. Sci.' and salary > 8000
```

## FROM Clause
The from clause lists the relations involved in the query 
- Find the Cartesian product instructor X teaches
```SQL
select * from instructor, teaches
```
- Generates every possible instructor – teaches pair, with all attributes from both relations.
- For common attributes (e.g., ID), the attributes in the resulting table are renamed using the relation name (e.g., instructor.ID)
	- Cartesian product not very useful directly, but useful combined with where-clause condition (selection operation in relational algebra)

