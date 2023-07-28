Transportability is the the process of translating the results of a study from one setting to another. 
- So using results from a study of one population and using it to make inferences about another population
	- In this way transportability goes hand-in-hand with [[External Validity]]. 

For transportability we differentiate between a source and a target population.

The star basically means we condition when s = 1

Direct transportability, aka naïve extrapolation, is when you directly apply your results to a somewhat similar population and say it is likely to be similar.


In [[Causal Inference]] we look at transportability via the transportability node (indicated by a solid square)
- Which shows that domains (populations) differ either in the distribution of background factors or causal mechanisms in the underlying[[Structural Causal Models]]. 
![[Pasted image 20230727140905.png]]
- So here it shows that the domain (population) differs in the Z variable

So the node is called S because it "selects" one of the two domains


## The Transportability Task
Is that we do have knowledge of the source domain, but want to have information about the target domain (is there the same causal effect)
- Not able to run experiment in target domain

Trivial transportability is when we can perform direct transportability (usually no unobserved confounders, since then we can just perform backdoor-adjustment)
- Unobserved confounder says we can perform the experiment in one domain, but not in the other


## S-Admissibility


S-admissibility only works if Z is pre-treatment
- If X has an arrow towards Z, then it is **post treatment** (Z comes after X (the treatment))
- If Z has an arrow towards Z, then it is **pre-treatment** (Z comes before X (the treatment))