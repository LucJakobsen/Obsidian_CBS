[[Logistic Regression]] is a [[Classification]] model, which is used to predict categorical variables (([[Dummy Variables]])).


We use the **logistic function** (also called **sigmoid function**) to convert the total contribution of variables/features into probability which shows how likely the event or behavior will occur


Before performing logistic regression we have to estimate the weights
- Basically we have to train the model because we don't know the weights


### Estimating the weights in Logistic Regression
Can be done in two ways:
1. [[Maximum Likelihood]]
2. [[Cross-entropy]]


In `sklearn`, the class `sklearn.linear_model.LogisticRegression` provides the following solvers:{‘lbfgs’, ‘liblinear’, ‘newton-cg’, ‘newton-cholesky’, ‘sag’, ‘saga’}, default=’lbfgs’

Algorithm to use in the optimization problem. Default is ‘lbfgs’. To choose a solver, you might want to consider the following aspects:
- For small datasets, ``‘liblinear’`` is a good choice, whereas ‘sag’ and ‘saga’ are faster for large ones;
- For multiclass problems, only ``‘newton-cg’, ‘sag’, ‘saga’`` and ``‘lbfgs’`` handle multinomial loss;
- ‘liblinear’ is limited to one-versus-rest schemes.
- ‘newton-cholesky’ is a good choice for n_samples >> n_features, especially with one-hot encoded categorical features with rare categories. Note that it is limited to binary classification and the one-versus-rest reduction for multiclass classification. Be aware that the memory usage of this solver has a quadratic dependency on n_features because it explicitly computes the Hessian matrix.

To evaluate the model in Python we look at the [[Classification Model Evaluation Metrics (Python)]]
