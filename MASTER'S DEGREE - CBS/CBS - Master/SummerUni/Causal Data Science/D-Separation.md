D-separation are a part of [[Directed Acyclic Graphs]] and are about manipulating the paths within [[Structural Causal Models]]. 

It allows us to say something about the structure of the graph and what they mean for the probabilistic elements of the graphs.

![[Pasted image 20230629153453.png]]

***Chain (A causes B causes C)*** basically saying: A and C are not independent, but if we can somehow hold B constant, then A and C are independent (we remove the relationship between A and C)

***Fork (B causes A and B causes C)*** basically saying: A and C are not independent, but if we can somehow hold B constant, then A and C are independent (we remove the relationship between A and C)

***Collider (A and C causes B)*** basically saying: A and C are independent, but if we can somehow hold B constant, then A and C are not independent (open/create a relationship between A and C)