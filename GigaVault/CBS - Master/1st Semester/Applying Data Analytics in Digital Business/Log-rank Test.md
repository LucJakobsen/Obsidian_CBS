Log-rank test is a statistical test used to compare the survival distributions of two or more groups.

It is used to test the [[Null Hypothesis]] of no difference between the survival functions of two or more groups.
- So it's used for [[Survival Analysis]]

To perform the log-rank test in STATA, use:
``sts test``

**Assumptions**: Proportional hazards
**Proportional hazards**: the hazard functions for any two individuals at any point in time are proportional, and does not change with time *t*

to check the proportional hazards we can make a loglog plot
![[Pasted image 20230430102955.png]]


in stata:
``stphplot, by()``

