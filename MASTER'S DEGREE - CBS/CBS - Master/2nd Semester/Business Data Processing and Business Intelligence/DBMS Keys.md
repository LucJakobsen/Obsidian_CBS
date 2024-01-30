Database Management System Keys are essential components in database design for [[Relational Databases]] and [[Database Management Systems (DBMS)]], to ensure data integrity and manage relationships between tables. 
- They help in uniquely identifying records, establishing links between tables, and ensuring data accuracy and consistency

### Types of DBMS Keys
1. **Primary Key**:
    - Uniquely identifies each record in a table.
    - Cannot have NULL values.
    - Each table can have only one primary key.
	    - Example: `StudentID` in a `Students` table.

2. **Foreign Key**:
    - Links records in one table to the primary key in another table.
    - Helps maintain referential integrity between tables.
    - Can have multiple foreign keys in a table.
	    - Example: `DepartmentID` in a `Students` table might be a foreign key referring to the `DepartmentID` primary key in a `Departments` table.

3. **Super Key**:
    - A set of one or more columns that uniquely identifies each record in a table.
    - Can be a single column or a combination of multiple columns.
    - Primary key and any unique keys are subsets of a Super Key.
    - Minimal Super Key (Super Key with no extraneous columns) is a candidate key.
    - Example: In a `Students` table, `StudentID`, `StudentID + FirstName`, `StudentID + LastName`, etc., are all Super Keys.

4. **Unique Key**:
    - Similar to a primary key, it uniquely identifies each record in a table.
    - Unlike a primary key, a table can have more than one unique key.
    - Can have NULL values.
	    - Example: `Email` in a `Students` table might be a unique key.

5. **Composite Key**:
    - Formed by combining two or more columns in a table.
    - Used when a single column is not sufficient to uniquely identify a record.
	    - Example: Combining `FirstName` and `LastName` in a `Students` table could form a composite key if each combination is unique.

6. **Candidate Key**:
    - Any column or set of columns that can be selected as a primary key.
    - A table can have multiple candidate keys, but only one can be chosen as the primary key.
	    - Example: In a `Students` table, both `StudentID` and `Email` might be candidate keys, but only one will be selected as the primary key.

7. **Surrogate Key**:
    - An artificial or synthetic key created to be a unique identifier.
    - Typically used when there is no natural primary or unique key.
    - Often an auto-incremented number.
	    - Example: An `ID` column added to a `Courses` table that does not have a natural unique key.

8. **Secondary Key**:
    - Used mainly for retrieval purposes rather than identifying records uniquely.
    - Allows efficient access to records based on the secondary key.
	    - Example: Indexing the `LastName` column in a `Students` table for faster search.

9. **Alternate Key**:
    - Any candidate key that is not selected as the primary key.
    - Still enforces uniqueness within the table.
	    - Example: If `StudentID` is the primary key in a `Students` table, an `Email` column could be an alternate key.