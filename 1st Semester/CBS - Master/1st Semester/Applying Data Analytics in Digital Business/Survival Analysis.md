Survival analysis is concerned with studying the time between entry to a study and a subsequent event. It is also called [[Time-to-Event]] analysis.

To perform survival analysis we can use [[Kaplan-Meier Method]].

Basic survival analysis is lacking statistical power and mostly used for preliminary research. 
- We can gain more by doing group comparison (kind of like an [[Experiment]] with two groups)
	- When we do group comparison we use [[Log-rank Test]] to determine if there's a difference between two groups


Like [[Logistic Regression]], survival analysis also deals with predicting a binary variable ([[Dummy Variables]]).
- But in survival analysis we are interested in the time to an event, rather than predicting based on multiple [[Independent Variable]].
- So we want to see how fast/slow it takes to reach an event and what variables influence this time

Survival analysis can be used to predict customer churn (basically customer loss)

Can also be used for e.g. a credit card company to measure the length of people keep using a credit card


In survival analysis, it is important to account for the [[Censoring|censor events]].

### Survival Analysis Methods
- [[Kaplan-Meier Method]]
- [[Cox Regression Model]]
