A DAG is a graph, comprised of nodes and edges (arrows). It is a type of [[Causal Diagram]]. 

The direction of an edge determines the relationship between the two nodes on either side.

DAGs allow us to check correlations between variables.

DAGs are useful because they allow us to encode conditional independence relationships ([[Statistical Independence]]) via [[D-Separation]]. 

**Example:**
![[Pasted image 20230629143948.png]]

**Nodes *V*:** variables in the model
**Directed edges *E*:** causal relationships in the model
**The dashed line (typically called *U*)** indicates that Z and Y are related by some sort of unobserved factor

**Graph Types:**
![[Pasted image 20230629143828.png]]

### Acyclicity Meaning
![[Pasted image 20230629145337.png]]