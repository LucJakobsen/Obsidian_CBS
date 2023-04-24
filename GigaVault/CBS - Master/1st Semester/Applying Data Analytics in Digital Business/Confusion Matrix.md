A confusion matrix, also known as a "contingency table" or "error matrix" is a table used to compare model predictions to true outcomes.

It summarizes the number of true positives, true negatives, false positives, and false negatives in a binary classification model. 

![[Pasted image 20230424192402.png]]

**True negative** = 7963 in the above case, meaning that the model correctly predicted 7963 lenders with low risk didn't violate their contract (they didn't make a default meaning that they did pay the money)

**True positive** = 24 in the above case, meaning that the model correctly predicted 24 lenders with high risk did violate their contract

**False positive** (aka [[Type 1 Error]]) = 32 in the above case, meaning that the model wrongly predicted 24 lenders with high risk that actually didn't violate their contract

**False negative** (aka [[Type 2 Error]]) = 32 in the above case, meaning that the model wrongly predicted 1497 lenders with law risk that actually did violate their contract



From this table, we can calculate various performance metrics such as accuracy, precision, recall, and F1-score:
- **Accuracy** = the proportions of customers that we correctly identified (how well the model estimated the true values)
	![[Pasted image 20230424192517.png]]
	- The higher the value, the better the model perfomance since better predictions

- **True Positive Rate** (Aka sensitivity or recall) = the proportion of violated cases that we correctly identified as high-risk (so how many true positive cases were correctly identified)
	![[Pasted image 20230424192817.png]]
	- The higher the value, the better the model perfomance

- **False Positive Rate** (Aka 1-specificity or Fall-out ) = the proportion of repaid cases that we correctly identified as high-risk (so how many true negative cases were correctly identified)
	![[Pasted image 20230424193113.png]]
	- The lower the value, the better the model performance