Do-calculus is essentially the process of mathematically eliminating the [[Do-operator]]s in theorems/functions. 



"Do-calculus" consists of three rules that can be applied to these graphs to manipulate and compute the effects of interventions:

1. **Rule 1 (Insertion/Deletion of Observations)**: If X does not influence Y, then intervening on X doesn't change the probability distribution of Y.
	- This rule allows us to add or remove variables from our diagrams, given they do not influence the causal effect between our variables of interest.
	
    
2. **Rule 2 (Action/Replacement of an intervention with an observation)**: If X does not influence Z, and we want to find the effect of intervening to set X to x, it doesn't matter whether we intervene on X before or after observing Z.
	- This rule means that the order of interventions doesn't matter if the variable being intervened upon doesn't influence the other variables in the set.
    
3. **Rule 3 (Insertion/Deletion or addition of interventions)**: If we are intervening to set X to x, and X is not influenced by any of the variables in the Z, then we can ignore other interventions on variables that are influenced by X when calculating the effect of our intervention on X.
	- This rule allows us to ignore other interventions on variables when they are influenced by the variable we are intervening on.