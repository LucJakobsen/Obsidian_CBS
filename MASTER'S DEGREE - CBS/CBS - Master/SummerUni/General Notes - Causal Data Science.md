### Lecture 1
Causality remains important as it may influence the results and interpretations we can gain from data. 

See e.g. the Google case (underpaying men vs. women)
- Average (mean) vs. adjust average (adjusted mean)
- You can find completely opposite answers based on how you view the data
- Data doesn't have all the answers, we require extra assumptions

There are no definite answers in causal inference --> it depends on the assumptions you have bring and have

Always consider if the data is equally distributed etc.


### Lecture 2
*Simplified history of AI*
1. Looking at Expert systems to create AI
2. Probability for AI --> leading to Bayesian networks etc.
3. Causality for AI

We, as humans, have a tendency to add a causality/causation effect when we see a correlation relationship.

Why is causation important?
*How can we prevent a future robot from trying to make the rooster crow at 3am in order to make the sun come up?*

There's correlation between the two, but the AI might think the rooster crowing will make the sun come up. And so it will do it at 3AM to have more sun / more efficient sun.


Current AI and ML techniques remain purely prediction-based
- To make them truly intelligent we need to take a step further (teach cause and effect)

The mathematical framework we use to teach ourselves and machines causality is [[Structural Causal Models]]. 

Causality is always an asymmetrical relationship
- So causation "goes one way"
- This is how causation differs from equations (equations are symmetrical and can be re-arranged)
	- This is not the case in causation
- The functions in causation can have any shape and form
	- Because in many contents we don't know how e.g. "gender" and "salary" relate to each other


### Lecture 3
- Causal paths and directed paths mean the same
- There can still be paths even when there is no causal path
![[Pasted image 20230704143521.png]]
	- So here we e.g. still see 2 paths, but only 1 causal path


- [[Confounders]] are usually forks, and [[Mediators]] chains

So in the example of Dynamic Pricing ---> Food Waste, mediators are in between, while confounders affect both but aren't between



### Lecture 4
##### Nearest neighbour matching
- for every observation we look for similar variables and try to match them (e.g. same value in z but different in x) 
- matching the observations together we can create a dataset where all the variables are the same in e.g. z but all differ in x
- you then compare treatment and control on these observations while one is constant (conditioned on)

- trade-off: nearest neighbour matching requires a lot of data
	- also, problem with overlap condition --> meaning sometimes there are no matches, so you need to settle for the next best

Also talked about [[Front-door Criterion]]. 

### Lecture 5
Focused on [[Experiment]]s and [[Experimentation]].


