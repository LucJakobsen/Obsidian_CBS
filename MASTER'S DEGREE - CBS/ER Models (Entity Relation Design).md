ER Models are high-level conceptual data models that are used in the initial design and analysis of [[Databases]]. 
- The ER model allows database designers to visualize the logical structure and relationships between different data elements without delving into physical storage details.
- It is used to represent the logical structure of database graphically
- It provides an overview of all the entities in one system and their relation to each other

These models are created after the conceptual design phase (see [[Relational Database Design]]), where the entities have been found

So i.e. the ER Models show the entities, their relations, and what type of relations they have.
- E.g. one-to-many, or many-to-one

### Three Elements of ER Models
1. ***Entity sets***
![[Pasted image 20230924113744.png]]

2. ***Attributes***
	- Represented via "diamond"
![[Pasted image 20230924113827.png]]
- 

3. ***Relationship sets***
- Can be either one-to-many or many-to-many
	- There are different notations to this
		- Either lines and arrows or the crowfoot (see below)
- Many-to-many relationships actually create a new entity between the two existing

**Examples:**
![[Pasted image 20230919130550.png]]
- (The two bottom ones show the same relationships as the ones above, just using the crowfoot notation instead)


![[Pasted image 20230924112207.png]]
- Each box represents one entity or one relation in the [[Relational Databases]] table
- A unique key/primary can be seen e.g. at student, where it is "ID"