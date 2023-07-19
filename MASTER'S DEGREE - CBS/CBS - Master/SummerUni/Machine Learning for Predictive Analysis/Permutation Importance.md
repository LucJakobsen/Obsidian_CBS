**Permutation importance** is a technique used to measure the importance of input features in machine learning. It provides insights into which features have the most significant impact on the model's performance. The idea behind permutation importance is to assess the model's performance when the values of a particular feature are randomly shuffled, thus breaking the relationship between the feature and the target variable.

It is typically used to evaluate [[Decision Trees]]. 

### Pros and Cons of Feature Importance
- Pros: it is a global measure and evaluates the importance of each feature in isolation.
- Cons: It doesn't capture potential interactions or dependencies between features.


### Feature Importance in Python
```
from sklearn.inspection import permutation_importance

result = permutation_importance(dtc, x, y, scoring="accuracy", random_state=100)

print("feature_importance: {}".format(result.importances_mean))

feature_importance_index = result.importances_mean.argsort()
print("feature_importance_index: {}".format(feature_importance_index))

feature_column = df_2.iloc[:, :-1].columns
print("feature_column: {}".format(feature_column))
```

