The backdoor-criterion is a set of rules to help identify a set of nodes to condition on that block all "backdoor paths" between X and Y.

Rules:  
1. X should not cause Z i.e. not be a descendant (no arrow from X to Z)  
2. Z blocks every path between X and Y that contains an arrow into X (every backdoor path)

The back-door criterion is essentially when we block all non-causal paths in a [[Causal Diagram]] and leaves only  the causal paths.
- So basically we "eliminate" [[Correlation]] and only leave [[Causation]]



It´s a way to deal with [[Confounding]]. 

If we lack data on the confounding variable, we cannot block the back-door path and instead must look at e.g. the [[Front-door Criterion]]. 
