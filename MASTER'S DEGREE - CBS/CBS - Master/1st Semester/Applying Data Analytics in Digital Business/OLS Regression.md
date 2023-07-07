Ordinal Least Squares (OLS) Regression is a [[CBS - Master/1st Semester/Applying Data Analytics in Digital Business/Regression|Regression]] method that estimates the relationship between one or more [[Independent Variable|independent variables]] and a [[Dependent Variable|dependent variable]].

It tries to answer the question: "What is the relationship between variable x and variable y"
- The relationship is assumed to be linear

Linear regression is all about predicting a continuous [[Dependent Variable]].
- Unlike [[Logistic Regression]] which is about predicting a [[Dummy Variables]]


The [[P-value]] will indicate whether a variable is useful for the prediction or not

The goal of OLS is to find the best-fit line over a scatter plot 

To see if the model actually is a good fit, we look at the value of the [[R-squared]].


![[Pasted image 20230417161702.png]]
**β**0 = the intercept on the y-axis
**β**1 = the slope
e = error
- Indicates that the prediction is not perfect and we try to account for it

I.e. the **β**'s are the regression coefficients. They are unknown to us, but we want to estimate them
- You interpret the coefficients by saying "1 unit change in x (e.g. original price) will mean 'coefficient number' change in y (e.g. sold price)"


The prediction error is minimized through measurement of the residual sum of squares (RSS)
- The smaller value of the RSS the better results
