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