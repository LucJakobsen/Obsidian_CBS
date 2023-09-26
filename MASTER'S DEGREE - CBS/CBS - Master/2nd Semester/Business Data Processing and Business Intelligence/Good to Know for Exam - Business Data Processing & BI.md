- An "entity" refers to a real-world object or concept that can be distinctly identified and needs to be represented in the database
- An entity has attributes, which describe the properties or characteristics of the entity. In a relational database, these attributes become the columns of the table. 
	- For example, an entity "Person" might have attributes like "FirstName", "LastName", "DateOfBirth", etc.

- "--" will make a comment

- Fact tables always have the one-to-many relation / many-sided
	- Dimension tables always have the one-sided

- Columns are called attributes
- Rows are called tuples
![[Pasted image 20230924104611.png]]

- As long as you identify entities correct, you make sure you remove duplicates, and apply normalization checks
	- Then your database should be performed alright

- Always create the parent table first

- If you EVER use a function (e.g. sum(price)) and combine it with a column outside the function, you HAVE to use "Groupby"
	- E.g.
		```SQL
		Select PID, SUM(Price)
		From ProductSale
		Group by PID
```


### Good things to include:
- Map the database via an [[ER Models (Entity Relation Design)]]
- Use views (see [[SQL Queries]]) to choose the data you want to include
- 