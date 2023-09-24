K-Nearest Neighbors (KNN) falls in the [[Supervised Learning]] family of algorithms. It is a [[Non-Parametric]] and [[Instance-based Learning]] algorithm.


The basic idea behind KNN is that we try to predict which category new data will fall in. We do this by comparing the features of the new variables with existing, similar variables (who have already been assigned a category). So if the features are similar to neighbors in category 1, the new variable will likely be put into category 1.
- We calculate the distance to similar variables


### Pros and Cons of KNN
**Pros**:
- Performs well with small-scale data
- High accuracy (good at interpolation)
- Insensitive to outliers
- No assumptions about data
- Works with numeric values, nominal values

**Cons**:
- Computationally expensive (so not good for large-scale data)
- Requires a lot of memory
- Might have poor performance if you have a lot of categorical variables, like [[Dummy Variables]]

**Small K or large K** (how many neighbors should we consider/use?)
(Usually you use between the top 5-15 K's)
- Small K
    - Creates many small regions for each class
    - May lead to non-smooth) decision boundaries and overfit
- Large K
    - Creates fewer larger regions
    - Usually leads to smoother decision boundaries (caution: too smooth decision boundary can underfit)


### Implementing KNN in Python
To implement KNN in Python we use:
``` Python
from sklearn.neighbors import KNeighborsClassifier
```

**Using KNN for classification:**
```Python
knn = neighbors.KNeighborsClassifier(
  n_neighbors=5, weights="uniform", p=2, metric="minkowski", algorithm="auto")

knn.fit(x_train, y_train)
```

