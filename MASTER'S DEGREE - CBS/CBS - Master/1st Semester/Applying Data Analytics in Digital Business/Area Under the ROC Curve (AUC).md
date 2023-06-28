The AUC is a metric that summarizes the overall performance of a [[Logistic Regression]] model. 

It ranges from 0.5 to 1, with a value of 0.5 indicating random chance and a value of 1 indicating perfect performance. 

Generally, a model with an AUC value above 0.7 is considered to be reasonably good.


The ROC Curve is created by plotting the true positive rate (TPR) against the false positive rate (FPR) (see [[Confusion Matrix]] for more info) at various threshold settings
- So different breaking points will give different TPR and FPR which values can be plotted in a graph

![[Pasted image 20230424194935.png]]

Everything under the curve is AUC. The larger the area, the better the model performance

![[Pasted image 20230424195010.png]]
