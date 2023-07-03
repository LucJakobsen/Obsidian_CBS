Belief Propagation also known as sum-product message passing, is a message-passing algorithm for performing inference in graphical models, such as [[Bayesian Networks]] and [[Markov Random Fields]].

The algorithm works by passing messages between nodes in the graph, and these messages contain information about the probability distributions of the nodes. 
- The nodes then use these messages to update their beliefs.

Essentially the network begins with a particular degree of belief in each possible statement about the nodes in the network. As new evidence is entered into the network—at any place in the network—the degrees of belief at every node, up and down the network, will change.


So kind of like explained here:
The networks are hierarchical, with arrows pointing from higher neurons to lower ones, or from “parent nodes” to “child nodes.” 

Each node sends a message to all its neighbors (both above and below in the hierarchy) about its current degree of belief about the variable it tracked
- If the message went from parent to child, the child would update its beliefs using [[Conditional Probability]]
- If the message went from child to parent, the parent would update its beliefs by multiplying them by a [[Likelihood Ratio]]
	- Applying these two rules repeatedly to every node in the network is called [[Belief Propagation]]. 
