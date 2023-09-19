Relational databases are a type of [[Databases]] that organizes data into structured tables with rows and columns.

Use tables to store data. The structure of these tables is defined by a schema.
	- Store most of the global data. Approximately 73% of total data according to TechRepublic.
	- Popular because of transaction handling.
	- Storage and retrieval are slower at cost of reliability.
	- Strongly typed and costly to change.


Relational databases can be either [[Operational Databases]] or [[Analytical Databases]].
- Typically we transform the operational database into an analytical, which will be suited for our analysis without affecting the stored operational data directly
	- The analytical database also has less "requirements" to follow/adhere to

### Creating Relational Databases
![[Pasted image 20230919122623.png]]
- The logical modeling part is where the relations are specified between the data entries


### Relational Database Principles
- Every row of data must have a unique identified (primary key), so that the specific row can be distinguished from others with similar data


Typically we want to split the database into various, relevant tables:
![[Pasted image 20230919130053.png]]

When we know the primary keys we can also "anonoymize" the data more and have other benefits by using ID's
![[Pasted image 20230919130115.png]]

To better understand the relationships between the entities in relational databases, we utilize [[ER Models (Entity Relation Design)]]. 
