Mutlicollinearity occurs when two or more [[Independent Variable|independent variables]] are highly [[Correlation|correlated]].

It makes the estimated coefficients ((see [[OLS Regression]]) very sensitive to noise in the dataset
- Can lead to inaccurate estimates which hurts the interpretability and predictive performance


Can usually be fixed by deleting one or more independent variables

Always check for multicollinearity before running regression!
![[Pasted image 20230417170514.png]]

- So the correlation coefficients should be below 0.7 to be acceptable

To know which variables to drop, use VIF ([[Variance Inflation Factors]])

