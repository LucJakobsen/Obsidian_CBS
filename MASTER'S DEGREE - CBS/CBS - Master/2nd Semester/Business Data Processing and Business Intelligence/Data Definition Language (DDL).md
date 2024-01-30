**Data Definition Language (DDL)** is a subset of [[Structured Query Language (SQL)]] that deals with the structure and schema of the database itself 
- Unlike [[Data Manipulation Language (DML)]]  which deals with the data contained within it.

In simpler terms, DDL is used to define and manage tables, indexes, and the overall structure of the database.
- DDL also deals with who is authorized to have access to what

### Primary DDL commands and their basic purposes:
1. **CREATE**: Used to create objects in the database. For instance, the `CREATE TABLE` command is used to create a new table.
    
    Example:
```SQL
CREATE TABLE Students (
    StudentID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50)
);
```

2. **ALTER**: Used to modify an existing database object. This can involve adding, deleting, or modifying columns in a table, or changing the data type of a column.
    
    Example:
```SQL
ALTER TABLE Students ADD Email VARCHAR(100);
```

3. **DROP**: Used to delete an object from the database, like a table, an index, or a view. Be cautious when using this command, as it removes data and structures permanently.
    
    Example:
```SQL
DROP TABLE Students;
```

4. **TRUNCATE**: Used to remove all records from a table but doesn't delete the table itself. It's a way to quickly clear out data without affecting the structure.
    
    Example:
```SQL
TRUNCATE TABLE Students;
```

5. **COMMENT**: Used to add comments to the data dictionary.
    
6. **RENAME**: Used to rename an object, such as a table.