Logistic Regression is a [[Regression]] and classification method. It involves [[Predictive Analysis|predicting]] a binary variable (([[Dummy Variables]])). 
- Unlike [[OLS Regression|linear regression]], which deals with predicting a continous [[Variable]].

***Typically:***
Y = 1 if "success"
Y = 0 if "failure"

- We seek to predict the probability of a "success" outcome of the [[Dependent Variable]] Y:
	- Predict the probability that Y = 1


***Logistic Function:***
![[Pasted image 20230424181707.png]]

### Interpreting Coefficients in Logistic Regression
- A change in a variable does not yield a linear change in the probability output by the model
	- Makes it difficult to communicate the precise meaning of a model coefficient

For this reason we interpret the coefficients using odds:
![[Pasted image 20230424190242.png]]

- In essence, using odds help us interpret the coefficients in a linear manner
- IMPORTANT: We take the log of the odds when using odds for logistic regression

![[Pasted image 20230424190711.png]]

### Assessing Logistic Model Performance
Since there's no R-squared for logistic regression we need another way to assess the performance

So instead, we can use the following:
- [[Confusion Matrix]]
- [[Area Under the ROC Curve (AUC)]] 