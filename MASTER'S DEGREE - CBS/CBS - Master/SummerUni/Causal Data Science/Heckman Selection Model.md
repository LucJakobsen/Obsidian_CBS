The Heckman selection model, is a statistical method that corrects for [[Selection Bias]]. The model is especially useful when the process of selection for a study or an observation isn't random, and this non-random selection might impact the results.

**Example:**
Imagine we want to know how much people earn, but we only have wage data for people with jobs. That leaves out all the people who don't work, maybe because they can't find a job or have chosen not to work. Their wages are technically zero, but if we just ignore them, we might overestimate the average wage. The Heckman selection model helps us adjust for this problem.


In more technical terms, the model involves two steps:
1. The first step models the probability of a subject being selected (in the job example, this would be the probability of a person having a job). This is done with a type of model called a probit model.
    
2. The second step models the outcome of interest (like wages), adjusted for the selection probabilities from the first step.
    

This way, the Heckman selection model helps us make better conclusions by accounting for selection bias.