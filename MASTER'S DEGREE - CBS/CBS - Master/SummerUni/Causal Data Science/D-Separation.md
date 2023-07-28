D-separation are a part of [[Directed Acyclic Graphs]] and are about manipulating the paths within [[Structural Causal Models]]. 
- So it's that one set of nodes is independent of another set of nodes given a third set

It allows us to say something about the structure of the graph and what they mean for the probabilistic elements of the graphs.
- Typically we start by creating a [[Causal Diagram]] and then test for independencies (unlike in [[Causal Discovery]]). 


## The D-separation Criterion
D-separation is related to [[Bayesian Networks]], more specifically three node networks who have the below junction (link) types:
![[Pasted image 20230629153453.png]]

1. ***Chain (A causes B causes C)*** basically saying: A and C are not independent, but if we can somehow hold B constant, then A and C are independent (we remove the relationship between A and C). A and C are correlated until we condition on B.
	- A familiar example is Fire --> Smoke --> Alarm
		- The fire  does not set off an alarm, so there is no direct arrow from Fire to Alarm. Nor does the fire set off the alarm through any other variable, such as heat.
	- The mediator B “screens off” information about A from C, and vice versa
		- Once we know the value of Smoke, learning about Fire does not give us any reason to raise or lower our belief in Alarm
			- (Fire and Alarm are conditionally independent, given the value of Smoke)


2. ***Fork (B causes A and B causes C)*** basically saying: A and C are not independent, but if we can somehow hold B constant, then A and C are independent (we remove the relationship between A and C)
	- B is often called a common cause or confounder of A and C. 
		- a confounder will make A and C statistically correlated even though there is no direct causal link between them
	- Example: Shoe Size <-- Age of Child --> Reading Ability. 
		- Children with larger shoes tend to read at a higher level. But the relationship is not one of cause and effect.

3. ***Collider (A and C causes B)*** basically saying: A and C are independent, but if we can somehow hold B constant, then A and C are not independent (open/create a relationship between A and C). So works opposite of chain and fork.
	- If we condition on B, we see a negative correlation between A and C. This is called [[Collider Bias]].
	- Example: Three features of Hollywood actors: Talent --> Celebrity <-- Beauty
		- both talent and beauty contribute to an actor’s success, but beauty and talent are completely unrelated to one another in the general population
