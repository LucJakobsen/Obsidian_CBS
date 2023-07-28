Cluster analysis is the task of grouping a set of objects/data points in such a way that objects/data points in the same group are more similar to each other than to those in other groups. A group is also called a **cluster**.

It is a popular [[Unsupervised Learning]] method widely used in business analytics, such as consumer segmentation and trading pattern recognition.

- There is no ground truth (or label) in data so cluster analysis is subjective!
- Cluster analysis itself is not one specific algorithm, but the general task to be solved. It can be achieved by various algorithms that differ significantly in their notion of what constitutes a cluster and how to efficiently find them.

They are several types of clustering methods, including:
- Partitioning clustering
- Hierarchical clustering
- Spectral clustering
- DBSCAN

In Python we typically use [[K-means Clustering]] for cluster analysis.