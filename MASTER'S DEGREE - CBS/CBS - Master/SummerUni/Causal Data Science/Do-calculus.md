Do-calculus is essentially the process of mathematically eliminating the [[Do-operator]]s in theorems/functions. 

Do-calculus only works in [[Directed Acyclic Graphs]]. 



"Do-calculus" consists of three rules that can be applied to these graphs to manipulate and compute the effects of interventions:

1. **Rule 1 (Insertion/Deletion of Observations)**: If X does not influence Y, then intervening on X doesn't change the probability distribution of Y.
	- This rule allows us to add or remove variables from our diagrams, given they do not influence the causal effect between our variables of interest.
	- P(y|do(x), z, w) = P(y|do(x), w)
		- So you remove the observed z
			- We delete an observation
	
    
2. **Rule 2 (Action/observation exchange)**: If X does not influence Z, and we want to find the effect of intervening to set X to x, it doesn't matter whether we intervene on X before or after observing Z.
	- This rule means that the order of interventions doesn't matter if the variable being intervened upon doesn't influence the other variables in the set.
	- P(y|do(x), do(z), w) = P(y|do(x), z, w)
		- So you replace the intervention z (do(z)) with an observed z
			- We replace an action with an observation
			- ![[Pasted image 20230718143256.png]]
			- can only be done if Y and Z are independent conditional on X and W
    
3. **Rule 3 (Insertion/deletion of actions)**: If we are intervening to set X to x, and X is not influenced by any of the variables in the Z, then we can ignore other interventions on variables that are influenced by X when calculating the effect of our intervention on X.
	- This rule allows us to ignore other interventions on variables when they are influenced by the variable we are intervening on.
	- P(y|do(x), do(z), w) = P(y|do(x), w)
		- We delete the intervention do(z)
			- We delete the action/intervention 



**Example EPL5:**
**Rule 1: Remove unnecessary pushes** 
Imagine that every time you pushed the red car, your little sister also pushed her green car. But you notice that whether your sister pushes her green car or not doesn't make any difference to how the red car moves. This rule says that you can forget about the green car push. So, even if you were trying to figure out what would happen when both you push the red car and your sister pushes the green car, you can just think about what happens when you push the red car.

**Rule 2: Replace similar pushes** 
Suppose now that sometimes, instead of you pushing the red car, your big brother pushes it. And you notice that when your big brother pushes the red car, it moves in the same way as when you push it. This rule says that when you're trying to figure out what happens when your big brother pushes the red car, you can think about what happens when you push the red car, because it's the same.

**Rule 3: Ignore sneaky pushes when they don't matter** 
Remember the sneaky cat? Sometimes it nudges the cars when you're not looking. But if you're trying to figure out what happens when you push the red car, and you know that the sneaky cat being around doesn't change anything about how your push moves the red car, then you can ignore the sneaky cat's nudges.

So, these three rules from our magic rule book help you to figure out what happens when you push the red car, even when other things might be happening, and even when you can't actually push the red car to see what happens. And that's a bit like how do-calculus works!