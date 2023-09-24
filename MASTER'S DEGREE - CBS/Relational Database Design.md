Relational database design refers to the process of organizing data into structured tables that can relate to each other, to efficiently store, retrieve, and manage data in a [[Databases]].
- So basically it's creating [[Relational Databases]]


There are three phases of a Relational Database design:
1. Conceptual Design
	- Requirements gathering
	- Identify purpose and entities/relations
	- Define business rules
	- Typical outcome is a rough Entity Relationship sketch

2. Logical Design
	- Define initial design further with annotations. i.e. ER model
	- Define relations between entities using Foreign Keys
	- Apply Normalization • Independent of the underlying platform

3. Physical Design
	- Implement Database in chosen Platform using [[Data Definition Language (DDL)]] statement
	- Datatypes, constraints and index decisions



To minimize data redundancy and avoid undesirable characteristics like insertion, update, and deletion anomalies, one can utilize [[Database Normalization]]. 

### Finishing Your Design
After Testing and Normalizing all the relations to third Normal form. There are steps that you need to perform: 
- Assign Unique Ids. For example, StudentId, InstructorId
- Define foreign key relations.
	- The attributes with a primary key role in the main table are added to the referenced table to connect.
	- This primary key of primary table is referred as Foreign Key in the detailed/referenced table
- Foreign key relations are drawn to connect different relations. This can result in creating new relations. For example connecting a student and course taken relation requires.
	- A new relation named takes
	- Studentid and courseid is the data in that table.
- Draw revised ER Model to keep an overview of entity structure.