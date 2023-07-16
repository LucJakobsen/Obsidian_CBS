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

### Lecture 6


### Lecture 7
[(225) CDSM20 – Keynote 1 - YouTube](https://www.youtube.com/watch?v=oTeygIetj34)

The lecture focuses on the more practical application of causal data science, illustrated through the example of the car rental company Lyft. Basically they are still at the second rung of the [[Ladder of Causality]]. They are performing a lot of interventions to deal with confounders etc.

Basically what they're trying to do is attempting to perform optimization, so they can maximize e.g. optimal level of incentives to increase the amount of drivers. 
- So a causal model with incentives and drivers
- So they examine causes and try to understand how they influence nodes so they essentially can optimize the investment into nodes

Lyft is experiencing problems with e.g. [[Confounding]]. 

To improve what happens in the Lyft marketplace, they perform interventions.:
![[Pasted image 20230716162158.png]]
- The interventions basically work by turning algorithms on/off
	- So a form of [[Experimentation]] - see if the algorithms are making a difference
	- They also do this via regions - so have treatment regions and control regions
	- They also want to perform variance reduction and reduce the error term --> gives a better estimate of the effect of the model
		- They want the effect to not have an effect on the particular baseline model

*Themes from the lecture*
- Confounding is less problematic because **we can intervene programmatically** Experimentation is a ubiquitous tool
	- So confounding is less problematic in business compared to academic
- Causal models provide the underpinning for effective decisions. We accumulate knowledge in formal models and automate decisions to the extent that we can
	- Not enough to estimate, we need to automate stuff
- Clearly defining goals and tradeoffs is paramount in a world of automated decision making
	- Else you might optimize the wrong stuff
- Predictive modeling adds value through helping us understand effect heterogeneity, reduce variance, and pool information across policies


Example DAG ([[Directed Acyclic Graphs]]) from Lyft:
![[Pasted image 20230716160414.png]]

Some-what summary of what was being done at Lyft:
![[Pasted image 20230716161610.png]]
![[Pasted image 20230716163926.png]]
