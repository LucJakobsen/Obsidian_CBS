``from sklearn.model_selection import cross_val_score``
K-fold Cross Validation is a procedure used to estimate the skill of the model on new data and in Python is related to the [[train_test_split]].

Basically we calculate the average model performance in both training and testing sets.

It allows each fold of data to be used at least once for testing and for training
![[Pasted image 20230706123711.png]]



``reg = LinearRegression()
``scores = cross_val_score(reg, x, y, cv=5, scoring="neg_mean_squared_error")