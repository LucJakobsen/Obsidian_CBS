Random forest is a representative of tree-based [[Bootstrap Aggregation]] algorithms. It incorporates of randomized feature selection when constructing decision trees. 

The logic behind the Random Forest model is that multiple uncorrelated models (the individual decision trees) perform much better as a group than they do alone

Random forest first randomly selects a **subset** of features, and then carries out the conventional split selection procedure within the selected feature subset. 
- This random feature selection/column subsampling can increase possibility of independence of weaker learners in the bagging, then increase the reduction in bias and variance.

Random forest usually builds trees without post-pruning.

The key hyperparameters of random forest are:
- **n_estimators**: The number of decision trees in the ensemble.
- **max_features**: The maximum number of features considered for splitting at each tree node. (perhaps most important!)
- **min_samples_split**: The minimum number of samples required to split an internal node.
- **min_samples_leaf**: The minimum number of samples required to consider a leaf node.
- **max_leaf_nodes**: The maximum number of leaf nodes the tree can have.
- **max_depth**: The maximum depth of the tree. If this setting is not specified, then nodes are expanded until all leaves are pure or until all leaves contain less than min_samples_split samples.