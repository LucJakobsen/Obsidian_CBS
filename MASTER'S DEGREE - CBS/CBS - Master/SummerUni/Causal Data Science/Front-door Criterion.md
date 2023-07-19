The front-door criterion are a set of rules that help identify what variables to condition on, when a certain variable mediates (chain) the path from the cause to the effect. 
- It allows us to control for confounders that we cannot observe

Related to when we can't measure all variables that we need for backdoor adjustment ([[Back-door Criterion]]). 

![[Pasted image 20230707140312.png]]

The front-door criterion requires that Z transmits the entire effect of X on Y ([[Mediators|mediates]] the effect)

#### Three conditions for the front-door criterion:
1. The middle variable (mediator) should be the main way x causes y.  
2. No unblocked back-door paths from x to the mediator  
3. All back-door paths from the mediator to y are blocked when we condition on x


The front-door criterion helps solve the identification problem ([[Structural Causal Models]]). 


#### How the adjustment it differs from back-door adjustment
It differs from the back-door adjustment in that we adjust for two variables (Smoking (x) and Tar (z)) instead of one, and these variables lie on the front-door path from Smoking to Cancer rather than the back-door path