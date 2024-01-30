A [[Structured Query Language (SQL)]] is a type of [[SQL Queries]]. JOIN combines records from two Tables
- A JOIN is used to locate related records from tables
- A query may contain zero, one or multiple JOIN operations

- There are following commonly used types of Joins
1. INNER JOIN
2. LEFT JOIN
3. RIGHT JOIN

### INNER JOIN
SELECTS records with the matching values in both tables
![[Pasted image 20230926143623.png]]

Example: 
```SQL
select * from student join takes on student.ID = takes.ID;
--or
Select * from student, takes where student.ID = takes.ID;
```


### LEFT (OUTER) JOIN
The left outer join preserves tuples only in the relation named before (to the left of) the left outer join operation
![[Pasted image 20230926143647.png]]

Example: Get a list of student who did not take a course 
```SQL
select * from student s left join takes t on s.id=t.id where t.id is null;
```


### RIGHT (OUTER) JOIN
The right outer join is symmetric to the left outer join
- Tuples from the right-hand-side relation that do not match any tuple in the left-hand-side relation are padded with nulls

![[Pasted image 20230926143754.png]]

Example: Get a list of student who did not take a course 
```SQL
select * from takes t right join student s on s.id=t.id Where s.ID is null
```

