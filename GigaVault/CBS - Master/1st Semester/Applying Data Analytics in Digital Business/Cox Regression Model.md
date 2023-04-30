Cox Regression Model is a popular statistical model used in [[Survival Analysis]] to investigate the relationship between one or more [[Independent Variable]] and the time to an event of interest

It is used to measure the [[Hazard Ratio]].

The cox regression model:
- Allows for prognostic factors, i.e. covariates 
- Explore the relationship between survival and explanatory variables
- Models and compares the hazards for different groups/factors (explanatory variables)
- Assumption: Survival curves with proportional hazards ((see [[Log-rank Test]]))

The cox regression model has stronger predictive power compared to the [[Kaplan-Meier Method]].


### Interpreting Cox Regression Coefficients Using [[Hazard Ratio]]

**Hazard ratio higher than one (>1)**
- The variable has a positive impact on whether an event happens

**Hazard ratior lower than one (<1)
- The variable has a negative impact on whether an event happens

***Example:***
![[Pasted image 20230430110743.png]]
