See [[Causal Diagram]]. 

Also sometimes referred to as "Data Generating Process (DGP)"
- The stuff on right side explains how the data is generated/created
	- So e.g. fx is a function that assigns values to x (in the example below)

**Examples:**
``z <-- fz(uz)
``x <-- fx(z,ux)
``y <-- fy(x,z,uy)

The f's denote the causal mechanisms in the model
- Are not restricted to be linear as in traditional structural equation models
The u's are background factors that are determined outside the model
Assignment operator (the arrow) captures asymmetry of causal relationships

y is usually the variable we care for - where we want to see change


We have to choose which variables we include in the model, and which we leave outside the model. 
- Exogenous vs. endogenous variables

To graphically represent Structural Causal Models we use [[Directed Acyclic Graphs]]. 


## Interventions in Structural Causal Models
- Interventions are essentially when we delete a causal model and replace it with a specific value

Interventions are essentially the [[Do-operator]]. 

![[Pasted image 20230706140733.png]]
- So we remove the line from z to x and replace it with x0
- E.g. 50% of people go to college in Denmark, what would happen if we removed the connection and tried to put everyone into focus

#### The Identification Problem (for interventions)
The identification basically mean we express something about the post-intervention world without actually having data on it.
- So e.g. we want to say something about if everyone went to college, without actually sending everyone to college
	- Because this might be too expensive, impractical, unethical, etc.

So identification is:
If we only have pre-intervention data (e.g. we can't force all people to smoke), we have to make a mapping between the world of pre-intervention and post-intervention data
![[Pasted image 20230706142424.png]]
P(Y|X) is basically [[Correlation]]s, while P(Y|do(X)) means the causal effect [[Causation]].

- Basically this is related to the problem/bias of [[Confounding]]. 

