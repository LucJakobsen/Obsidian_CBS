Selection bias is a kind of distortion that can occur in research or studies when the participants, data, or situations selected for analysis aren't representative of the larger population or phenomenon being studied. 
- So basically it's like picking only the green M&Ms from a bag and then saying all M&Ms are green
	- it's when we make a mistake because we only looked at part of what we should have.


This can skew the results and make them less accurate or applicable to the general population.
- Reducing the [[External Validity]]

If you don't take sample bias into account properly, you risk drawing the wrong conclusions


**Example:**
![[Pasted image 20230723175359.png]]

So the causal diagram shows that minority status may have an effect on whether you are stopped and may have an effect on the use of force (which is what we are investigating)
- but stopping might also be connected to force via an unobserved variable - leading to selection bias
- since all our data is based on people who have been stopped we are conditioning on stopping
	- which is problematic as it is a collider - opens path between minority and force (can't be sure if it's a causal effect or the collider structure)


## Recovering from Sample Bias
We can recover from sample bias so that we can still work with a selected sample but still infer some generalizations about the population from our research. 

We can do this in more traditional ways, such as [[Selection Propensity Score]], or [[Heckman Selection Model]], but this carries with it certain assumptions.

Or we can use [[Directed Acyclic Graphs]] / [[Causal Diagram]]s, which are without assumptions.
- We do this by including a selection node (S), and the variables which have an influence on the selection have an arrow towards S
![[Pasted image 20230723181909.png]]
- The selection node can only receive arrows, it can't send any
- But even this is not possible if the selection node is somehow connected to the output variable
- Sometimes we can combine biased and unbiased data to help recover from [[Selection Bias]]

