Relational databases are a type of [[Databases]] that organizes data into structured tables with rows and columns.
- The relations between various tables are handled via what is known as [[DBMS Keys]]. 

![[Pasted image 20230920131916.png]]

Use tables to store data. The structure of these tables is defined by a schema.
	- Store most of the global data. Approximately 73% of total data according to TechRepublic.
	- Popular because of transaction handling.
	- Storage and retrieval are slower at cost of reliability.
	- Strongly typed and costly to change.


- For designing Relational Databases, see [[Relational Database Design]]

#### Why are Relational Database Management Systems Popular?
They are popular because the key transaction support ACID
- **Atomicity**
	- It's all or nothing. If something goes wrong during a data action, everything goes back to the way it was.
- **Consistency**: 
	- They make sure data stays correct and follows the rules both before and after any action.
- **Isolation**: 
	- Many things can happen at the same time without mixing up
		- I.e. when multiple operations (like saving or changing data) are happening at the same time in the database, each operation is kept separate from the others
	- Ensures operations don't interfere with each other
- **Durability**: 
	- Once you save something, it stays saved, even if there's a problem later on.
	- So if the system fails, it will still go back to the last save where all was good

Relational databases can be either [[Operational Databases]] or [[Analytical Databases]].
- Typically we transform the operational database into an analytical, which will be suited for our analysis without affecting the stored operational data directly
	- The analytical database also has less "requirements" to follow/adhere to

### Creating Relational Databases
![[Pasted image 20230919122623.png]]
- The logical modeling part is where the relations are specified between the data entries

### Interacting with Relational Database Management Systems
To interact with relational database management systems we use [[Structured Query Language (SQL)]]

### Relational Database Principles
- Every row of data must have a unique identified (primary key), so that the specific row can be distinguished from others with similar data

Typically we want to split the database into various, relevant tables:
![[Pasted image 20230919130053.png]]

When we know the primary keys we can also "anonoymize" the data more and have other benefits by using ID's
![[Pasted image 20230919130115.png]]

To better understand the relationships between the entities in relational databases, we utilize [[ER Models (Entity Relation Design)]]. 


### Data Abstraction in Relational Databases
- Physical level: describes how a record (e.g., instructor) is stored.
- Logical level: describes data stored in database, and the relationships among the data. 
	type instructor = record 
		ID : string; 
		name : string; 
		dept_name : string; 
		salary : integer;

- View level: application programs hide details of data types. Views can also hide information (such as an employee’s salary) for security purposes.

So, in simpler terms:
- **Physical level**: How the data is stored on the computer.
- **Logical level**: What data is there and how it's organized.
- **View level**: How specific users or apps see the data, with unnecessary details hidden.

![[Pasted image 20230920134346.png]]
