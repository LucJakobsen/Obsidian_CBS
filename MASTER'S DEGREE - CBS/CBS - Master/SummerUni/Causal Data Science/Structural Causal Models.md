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
See [[Interventions in Structural Causal Models]]

