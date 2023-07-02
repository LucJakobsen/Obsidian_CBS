Bayesian Networks is a graphical model that represents the probabilistic relationships among a set of variables.

They rely heavily on [[Bayes' Rule]] to solve [[Inverse Probability]]. Basically we tell the computer the [[Forward Probability]], and the computer tells us the inverse probabilities when needed

The networks are hierarchical, with arrows pointing from higher neurons to lower ones, or from “parent nodes” to “child nodes.” 

Each node sends a message to all its neighbors (both above and below in the hierarchy) about its current degree of belief about the variable it tracked
- If the message went from parent to child, the child would update its beliefs using [[Conditional Probability]]
- If the message went from child to parent, the parent would update its beliefs by multiplying them by a [[Likelihood Ratio]]
	- Applying these two rules repeatedly to every node in the network is called [[Belief Propagation]]. 



### Bayesian Network uses:
- Speech-recognition software
- Spam filters
- Weather forecasting
- Evaluation of potential oil wells
- The Food and Drug Administration’s approval process for medical devices
- Skill ranking in Xbox video games
- etc.