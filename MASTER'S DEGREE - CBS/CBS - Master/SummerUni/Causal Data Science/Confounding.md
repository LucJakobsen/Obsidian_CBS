In statistics and research, confounding occurs when the effect or association between an [[Independent Variable]] and a [[Dependent Variable]] is mixed up with the effect of a third variable, known as a [[Confounding Variable]] or confounder.

The term “confounding” originally meant “mixing” in English. 

In [[Causal Diagram]]s, we typically see these variables when we see a third variable influencing the relationship between the other variables, by influencing both of them.
![[Pasted image 20230703131206.png]]
For example, if we are testing a drug and give it to patients who are younger on average than the people in the control group, then age becomes a confounder

## Confounding Bias
Confounding bias is basically that there might a path ([[Correlation]]) between variables that isn't causal
![[Pasted image 20230706143825.png]]

So here there's a causal path x -->, but there is also a confounding path going x - w - z - y

### Dealing with Confounding
However, if we have measurements of the third variable, then it is very easy to deconfound the true and spurious effects. 
- For instance, if the confounding variable Z is age, we compare the treatment and control groups in every age group separately
- Basically we condition on a variable to "block"/change paths 

This is typically called "controlling for Z" or "adjusting for Z", and is done like this:
- Take an average of the effects, weighting each age group according to its percentage in the target population

So e.g. in the example above we can either condition on w or z

- Basically we want to fulfil the [[Back-door Criterion]]
