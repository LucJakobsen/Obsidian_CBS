An experiment is a single test (or series of test-runs) of an activity under control by the researcher, where one or more [[Variable|variables]] are manipulated to observe the effect on another variable - while also accounting for [[Extraneous Variable|extraneous variables]] and [[Confounding Variable|confounding variables]].

I.e. it is a method used to study [[Causation]].
- A measure used estimating the causal effect could e.g. the [[Average Treatment Effect (ATE)]]

In an experiment, the goal is to isolate the [[Independent Variable|independent variable]] and determine its effect on the [[Dependent Variable|dependent variable]]. 

Experiments can either be [[Within-subject Experiment|within-subject]] or [[Between-subject Experiment|between-subject]].


#### Experiment Design
Experiments can be designed in different ways, for example it can follow a [[Full Factorial Design]] or a [[Fractional Fractorial Design]].


Furthermore, experiments can be either [[Lab Experiment]] or a [[Field Experiment]]. However, they can also be a [[Scenario-based Lab Experiment]]

### Guidelines for Designing an Experiment
1. Recognition & Statement of Problem
	- Clearly define the research question and the problem that the experiment seeks to address.
2. Selection of the Response Variable(s)
	- Identify the outcome(s) or [[Dependent Variable|response variable(s)]]' that will be measured to assess the effect of the treatment or intervention.
3. Choice of Factors, Levels, and Ranges
	- Determine the independent variables or factors that will be manipulated in the experiment, along with the levels or ranges of these variables.
4. Choice of Experimental Design
	- Select an appropriate experimental design that allows for proper control of extraneous variables and minimizes potential sources of bias, such as randomization or blinding.
		- Choose [[Within-subject Experiment]] or [[Between-subject Experiment]]
5. Performing the Experiment
	- Conduct the experiment and collect the necessary data.
		- Avoid [[Confounding Procedures]]
6. Statistical Analysis of the Data
	- Analyze the data using appropriate statistical methods to test the hypothesis and assess the significance of the results.
7. Drawing Conclusions, Recommendations
	- Based on the results of the experiment, draw conclusions and make recommendations for future research or practical applications.


##### Example reasons for running an experiment:
![[Pasted image 20230313214637.png]]

### Practical Considerations for Experimental Design
- Most A/B tests in practice do not show such spectacular results as suggested in Thomke’s HBR piece
- Sometimes, just the awareness of taking part in an experiment can change people’s behavior, even if no treatment is administered (Hawthorne effect)
- We can test whether treatment and control group is balanced with respect to observable covariates, but be aware of type-1 error
- You need to make sure that there is sufficient sample size in each treatment arm (power calculation)
- Effects can occur in clusters
	- In this case, treated an untreated units are not independent of each other ⇒ SUTVA (stable unit treatment value assumption) violation
- Averages can hide treatment effect heterogeneity
- Consider to pre-register your experiments