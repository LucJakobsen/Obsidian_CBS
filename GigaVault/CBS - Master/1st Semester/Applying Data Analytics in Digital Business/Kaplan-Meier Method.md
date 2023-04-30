The Kaplan-Meier method is a non-parametric statistical technique used to estimate the survival probability of a [[Population]] over time in the presence of [[Censoring|censored]] observations. 


It is commonly used in [[Survival Analysis]] to estimate the survival function, which represents the probability of an event occuring over time ([[Time-to-Event]]).



We check the status of the subjects each month, so at start of each month subject status can change
- That's why we see the stair-like shape
![[Pasted image 20230430094126.png]]
y-axis = cumulative survival rate
- 1 = 100% survival rate (all subjects alive)
- 0 = 0% survival rate (all subjects died)
x-axis = timeline

Fraction survival = represents the number of survival at a specific time
Hazard = represents the instantaneous risk of an event at a given time

From the graph we can find median survival rate when cummulative surival = 0.5


![[Pasted image 20230430100905.png]]

If the slope of the curve is steep = survival rate is low
If the slope of the curve is falt = survival rate if high

Slope is not linear, changes over time


### Limitations of Kaplan-Meier
- Mainly descriptive
	- Survival rate and survival rate between multiple groups
	- Lack of prediction power
- Doesn't control for covariates ([[Independent Variable]])
- Requires categorical predictors