**Data Manipulation Language (DML)**, also known as Query Language, is a subset of [[Structured Query Language (SQL)]] focused on the retrieval, insertion, modification, and deletion of data within a database. 
- Unlike [[Data Definition Language (DDL)]], which deals with the structure and schema of the database itself 

In other words, while DDL (Data Definition Language) deals with the structure and design of a database, DML handles the actual data inside those structures.

### Primary DML commands and their basic purposes:
1. **SELECT**: Used to retrieve data from one or more tables. This is probably the most frequently used SQL command. With it, you can specify criteria to get just the data you want.
    
    Example:
``` SQL
SELECT FirstName, LastName FROM Students WHERE StudentID = 5;
```

2. **INSERT**: Used to add new records (rows) into a table.
    
    Example:
``` SQL
INSERT INTO Students (StudentID, FirstName, LastName) VALUES (6, 'John', 'Doe');
```

3. **UPDATE**: Used to modify existing records in a table based on certain criteria.
    
    Example:
``` SQL
UPDATE Students SET Email = 'john.doe@example.com' WHERE StudentID = 6;
```

4. **DELETE**: Used to remove existing records from a table based on certain criteria. It's essential to use this command with caution, as deleting data is often irreversible.
    
    Example:
``` SQL
DELETE FROM Students WHERE StudentID = 6;
```