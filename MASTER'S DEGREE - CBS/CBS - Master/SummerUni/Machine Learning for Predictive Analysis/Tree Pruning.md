There are two techniques used in [[Decision Trees]] to prevent [[Overfitting]] and improve the generalization ability of the model: pre-pruning and post-pruning.

**Pre-pruning** (or **early stopping**) = used during the construction of a decision tree. It involves setting conditions to stop the tree's growth early, preventing it from becoming too deep or complex.

Some commonly used pre-pruning techniques include:
- **min_samples_split**: The minimum number of samples required to split an internal node.
- **min_samples_leaf**: The minimum number of samples required to consider a leaf node.
- **max_leaf_nodes**: The maximum number of leaf nodes the tree can have.
- **max_depth**: The maximum depth of the tree. If this setting is not specified, then nodes are expanded until all leaves are pure or until all leaves contain less than min_samples_split samples.

Through the application of pre-pruning techniques, the decision tree construction process is able to terminate early if any of the specified conditions are satisfied.


**Post-pruning** (or simply **pruning**) is a technique used after the decision tree has been fully grown. Its purpose is to simplify the tree structure and enhance generalization by eliminating or collapsing unnecessary nodes or branches.
- **Cost complexity pruning** is a commonly used post-pruning technique

Post-pruning helps reduce the complexity of the decision tree, making it less sensitive to noise or irrelevant features in the training data. It promotes a more generalized and interpretable tree without sacrificing too much predictive performance.