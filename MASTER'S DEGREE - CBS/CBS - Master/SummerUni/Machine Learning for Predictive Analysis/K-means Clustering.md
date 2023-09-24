K-means clustering is a method for [[Cluster Analysis]], which is a task of grouping data points within groups (clusters) based on their similarities.

In K-means clustering, the K means the number of clusters we want to have
	- (Unlike in [[K-Nearest Neighbors (Python)]], where K means number of neighbors)

**Basic Idea:**
![[Pasted image 20230725111807.png]]

The basic idea is we make a random guess and then assign the nearby values to clusters.
- You then keep re-calculating the guess-points until they no longer move - indicating that the clusters are now final


## K-means Clustering in Python
To implement the k-means clustering, we can use the `KMeans` class from the `cluster` module in the `sklearn` library:
``` Python
from sklearn.cluster import KMeans
import numpy as np

random_seed = 100
num_clusters = 2
kmeans = KMeans(n_init="auto", n_clusters=num_clusters, random_state=random_seed)
kmeans.fit(x)
```

### Finding the Optimal K
There are several data-driven methods available to determine the optimal value of K in K-means clustering. One of the popular techniques is known as the **elbow method**. Essentially, for each value of K, we calculate the within-cluster sum of squares (WSS or WCSS) value. As the value of K increases, the WCSS value begins to decrease. The largest WCSS value occurs when K=1, representing a single cluster.

In practice, we can use `KElbowVisualizer` from `yellowbrick.cluster` to implement the elbow method to find the optimal number of clusters by fitting the model with a range of values.
``` Python
from yellowbrick.cluster import KElbowVisualizer

kmeans_search = KMeans(n_init="auto")

# specifying the range of k's we want to search, here 2-10
visualizer = KElbowVisualizer(kmeans_search, k=(2, 10))
visualizer.fit(x)
visualizer.show()
plt.show()
```

