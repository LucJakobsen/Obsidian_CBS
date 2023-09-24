Decision trees are essentially a series of questions which we use to evaluate decisions based upon. They're basically a series of if-else statements. 
They can be considered a white-box model [[Black Box and White Box Models]]

A drawback about decision trees is that they are prone to [[Overfitting]]. 
- To combat this there is also models using [[Ensemble Learning]] such as [[Random Forests]]. 

- A **tree** is a directed, connected graph with one **root node**.
- Every other node has a single predecessor (parent) and no or more successors (children).
- Nodes without successors are called **leaves**.
- All nodes are connected by **edges**.
![[Pasted image 20230718112421.png]]
- Leaves (leaf nodes / terminal nodes), are typically what we end up doing. So they're at the bottom of the decision tree.
- Root nodes are the top of the decision tree and what we start with. 

![[Pasted image 20230718112703.png]]
- The **depth of a node** is the number of edges on the path to the root.
- The **height of the whole tree** is the number of edges on the longest path from the root to any leaf.


A key concept for decision trees is [[Information Entropy]], which is used to determine the amount of impurity in a node. 

To prevent overfitting and improve generalization we can perform [[Tree Pruning]]. 


### Decision Trees in Python
**Visualizing the tree**
We can use `export_graphviz` to generate tree graph

```Python
from sklearn.tree import export_graphviz
import pydotplus
from IPython.display import Image

dot_data = export_graphviz(
    dtc,
    out_file=None,
    feature_names=col_select_category[0:-1],
    class_names=label_names,
    filled=True,
    rounded=True,
    special_characters=True,
)

# Draw graph 
graph = pydotplus.graph_from_dot_data(dot_data)

# Show graph
Image(graph.create_png())
```

### Evaluating Decision Trees
Evaluating decision trees is done via looking at variable importance and/or [[Permutation Importance]]. 



