- Check distribution before choosing algorithms/models for prediction
- 

- Start with descriptive statistics
- Check different scatter plots to choose best fitting for linear regression
	- Calculate correlation coefficient to help decide
- The random seed from canvas should be put in the random_state for [[train_test_split]]

- Use ``df.isnull()`` to check for missing values
	- ``df.isnull().sum()`` will provide an overview of the various columns´ missing data

- For [[Logistic Regression (Python)]] we typically benchmark with random guess (50%)


- Check if data sample has to be resampled
- Always check if the index is weird or somehow not in order
- Might be good to optimize parameters using cross-validation etc.
- .flatten() ensures that it is a vector - might be useful across different versions of Python to avoid errors


***Hyperparameter Tuning for Decision Trees***:
```
parameters={"splitter":["best","random"],
            "max_depth" : [1,3,5,7,9,11,12],
           "min_samples_leaf":[1,2,3,4,5,6,7,8,9,10],
           "min_weight_fraction_leaf":[0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9],
           "max_features":["auto","log2","sqrt",None],
           "max_leaf_nodes":[None,10,20,30,40,50,60,70,80,90] }

from sklearn.model_selection import GridSearchCV

clf = GridSearchCV(``--REGRESSIONMODEL HERE--``, parameter_space, cv=3, n_jobs=4)
clf.fit(x_train, y_train) 
```
- Might have to specify scoring as well by specifying ``criterion='mse'`` 


Ensemble trees does not always ensure the most accurate models, but will guarantee a more robust model

We typically don't do post-pruning in ensemble models

For small datasets, single decision trees might sometimes outperform ensemble models such as random forest etc.