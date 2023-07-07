Causal discovery rely on the [[D-Separation]] criterion we have already encountered and try to infer a compatible [[Directed Acyclic Graphs]] from the conditional independence relationships found in the data


So normally we first create the [[Causal Diagram]] and then perform the independence tests ([[Inconditional Independencies]]). However in Causal Discovery we start with the independence tests.
![[Pasted image 20230706135340.png]]

So in causal discovery this happens:
The conditional independence relationships on the right can actually be used to learn the graph on the left from data

So we first go to the data without a causal model, and then try to create a model based on the data

Causal discovery does not invalidate the “no causes in, no causes out”

## Drawback of Causal Discovery
***You can not distinguish between forks and chains [[D-Separation]], so this can't be checked in the data***


