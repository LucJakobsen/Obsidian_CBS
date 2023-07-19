Instrumental variables are a type of variable used in statistical and econometric analysis to estimate causal ([[Causation]]) relationships when there might be unobserved [[Confounding Variable]]s.

In an ideal [[Experiment]], we'd control all confounding variables to isolate the causal effect of one variable on another. However, in many real-world scenarios, it's often impossible to run controlled experiments, and observational data may be subject to hidden confounding variables.

Here, an instrumental variable (IV) can help. An IV is a variable that is:

1. **Correlated with the [[Independent Variable]] (or the explanatory variable)**: The IV should be associated with the variable whose effect you're trying to measure.
    
2. The instrumental variable should not be linked with other hidden things that could affect the dependent variable, other than through its effect on the independent variable.



**Example:**
Suppose we want to estimate the effect of education (the independent variable) on income (the dependent variable), but we're concerned there may be hidden confounding variables (like natural ability or socioeconomic background) that both influence a person's level of education and their potential income.

If we find an instrumental variable, like a policy change that increased educational access in certain regions, it could be used to isolate the effect of education on income. The idea is that the policy change is correlated with the level of education (people in regions where access was increased are likely to have higher education) but doesn't directly influence income (other than through its effect on education).