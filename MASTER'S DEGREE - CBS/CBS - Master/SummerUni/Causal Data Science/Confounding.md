In statistics and research, confounding occurs when the effect or association between an [[Independent Variable]] and a [[Dependent Variable]] is mixed up with the effect of a third variable, known as a [[Confounding Variable]] or confounder.

The term “confounding” originally meant “mixing” in English. 

In [[Causal Diagram]]s, we typically see these variables when we see a third variable influencing the relationship between the other variables, by influencing both of them.
![[Pasted image 20230703131206.png]]
For example, if we are testing a drug and give it to patients who are younger on average than the people in the control group, then age becomes a confounder


### Dealing with Confounding
However, if we have measurements of the third variable, then it is very easy to deconfound the true and spurious effects. 
- For instance, if the confounding variable Z is age, we compare the treatment and control groups in every age group separately

This is typically called "controlling for Z" or "adjusting for Z", and is done like this:
- Take an average of the effects, weighting each age group according to its percentage in the target population

