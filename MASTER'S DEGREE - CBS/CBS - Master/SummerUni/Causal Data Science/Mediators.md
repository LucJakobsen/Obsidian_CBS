In causal data science and for [[Causal Diagram]]s, mediators are the middle variable in a chain (see [[D-Separation]]). 


It's is a variable that helps explain the relationship between an [[Independent Variable]] (the cause) and a [[Dependent Variable]] (the effect). 

In other words, a mediator is a variable that lies on the causal path, where it transmits ([[Mediation|mediates]]) the effect from the independent variable to the dependent variable.

![[Pasted image 20230707140312.png]]

So here Z is a mediator


We want to ask certain typical questions about a mediator: Does it account for the entire effect?
- Conditioning on a mediator is incorrect if we want to estimate the total effect of one variable on another
	- But can be needed/useful to determine the [[Direct Effects]]