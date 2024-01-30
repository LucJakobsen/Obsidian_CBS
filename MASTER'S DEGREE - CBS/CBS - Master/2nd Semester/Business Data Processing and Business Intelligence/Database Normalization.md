Database normalization is a systematic approach to designing [[Relational Databases]], and is therefore a key part of the [[Relational Database Design]].
- The main aim is to organize a database into well-structured, smaller tables and define relationships between them

Basically it's about decomposing a table into less redundant (and smaller) tables but without losing information.


So the goal is to derive a set of schemas each of which are in “good form”
- Allow storing information without un-necessary redundancy
- Allow information retrieval easily and completely

#### The approach works in the following manner:
- Find Good Form for tables
- Decompose if needed to further tables
- Evaluate again
- The decomposition should not result in Loss of Information.


## Normal Forms
The process is carried out in stages, and each stage is called a "normal form." There are several normal forms, each with an increasing level of normalization:

1. **First Normal Form (1NF)**
    - Every column contains atomic, indivisible values (cannot be broken into smaller parts)
    - No repeating groups or arrays are allowed.
    - Each entry in a column is of the same data type.
![[Pasted image 20230924130538.png]]

**Issues with First Normal Form (1NF):
- Data anomaly
	- The data is heavily duplicated
- Insertion anomaly
	- Will create null values if we want to e.g. insert a new phone number without a course
- Update anomaly
	- Changing e.g. the mobile-phone of one person, you have to find every unique ID and update it there too accordingly
- Deletion anomaly
	- Deleting one attribute will delete the entire entry/row/tuple

2. **Second Normal Form (2NF)**
    - The table is in 1NF.
    - All non-key columns are fully functionally dependent on the primary key.
    - Eliminates ***partial dependencies*** on a composite primary key.

3. **Third Normal Form (3NF)**
    - The table is in 2NF.
    - There are no ***transitive dependencies***, where one non-key column depends on another non-key column.
    - Every non-key attribute is non-transitively dependent on the primary key.



There are also other forms, but these are rarely used:
4. **Boyce-Codd Normal Form (BCNF)**
    - A stricter version of 3NF.
    - Every determinant is a candidate key.
    - Addresses certain anomalies not handled by 3NF.

5. Fourth Normal Form (4NF)**
    - The table is in BCNF.
    - Multi-valued dependencies are absent.
    - No more than one independent many-to-many relationship exists within the same table.

6. **Fifth Normal Form (5NF)**
    - The table is in 4NF.
    - Deals with join dependencies.
    - Every join dependency in the table is a consequence of its candidate keys.