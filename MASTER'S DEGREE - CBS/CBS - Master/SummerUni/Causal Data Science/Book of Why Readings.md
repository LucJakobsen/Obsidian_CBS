#### Main Question Addressed in the Book:
*How can machines (and people) represent causal knowledge in a way that would enable them to access the necessary information swiftly, answer questions correctly, and do it with ease, as a three-year-old child can?*

***Data do not understand causes and effects; humans do.***

### Introduction
The first section of the book introduces the science of "[[Causal Inference]]" and [[Causation]].

It basically talks about the understanding behind cause and effect, and goes a bit back in time to explain how understanding what causes something and that changing the cause will alter the result has been the backbone of science and human progression. 

It also tells us how there has not really been a mathematical language for causation for quite a while in statistics (it basically used to be prohibited), but it's important to have so we can answer questions of ***why*** something happens - something which data by itself can't. 

It's basically about being able to isolate the [[Dependent Variable]] from [[Extraneous Variable|confounding and extraneous variables]]. 

We want to predict effects of an intervention (treatment) without enacting it.

Also says some stuff about [[Counterfactual Reasoning]] - dealing with "what ifs"

In essence, what makes humans so great and able to push forward in science is that we can ask the "what ifs" and try to answer them. AI e.g. can't do this unless it has data to back it up or data to which what ifs could happen (I think?)
- If we want AI to do this we need to give them a causal model

### Chapter 1
This chapter starts with a bit of a look at human evolution and how we have developed to have causal inference and need for causal explanations - which make up the bulk of our knowledge.

Causality helped us evolve faster. We can imagine causal relations and their consequences - we can therefore plan things.

When we plan we make mental models and see how factors might influence the results (what effect do they cause).

**So basically the main argument in the chapter is that our ability to imagine things have made us unique and able to develop so quickly - and machines can't do this yet**

The chapter also introduces us to the [[Ladder of Causality]]. 

With the ladder in mind they explain how machines and AI with deep neural networks are still at step 1. They make associations based on their data but can't figure out things on their own - if the machine needs to act differently in a situation these reactions have to be added to it before.

[[Experiment|Experiments]] are used to predict the results of interventions (manipulate [[Independent Variable]] to see causal effect on [[Dependent Variable]])

The chapter goes on to talk about a sort of "mini" [[The Turing Test]], by trying to make a machine think about causal events related to a single story. 

***<If we want our computer to understand causation, we have to teach it how to break the rules>***

Ends a bit with saying that probability is not enough, especially because of stuff like [[Confounding Variable]]s which can influence the results etc. So causation is important to understand if we really want advanced AI and machines.

### Chapter 2
This chapter starts out with a bit of history about of how the [[Normal Distribution]] came to be, and how it is linked to the [[Central Limit Theorem]]. The historic explanation (in relation to Sir Francis Galton) then goes on to link these to the concept of [[Regression to the Mean]].

This then leads to the birth of the word [[Correlation]]: "*Galton started using a new word for this kind of relationship: height and forearm length were “co-related.” Eventually, he opted for the more normal English word “correlated*"

Galton continues his research on linkage between father and son genetics (e.g. height), leading to the [[CBS - Master/1st Semester/Applying Data Analytics in Digital Business/Regression|Regression]] line and the finding that correlation does not mean causation. Later his disciple, Karl Pearson, created the correlation coefficient.

So basically, Galton proved that regression to the mean does not require a causal explanation, and Pearson then took this and said "causality isn't needed and it can't be proved".

But Pearson discovered quite a few problems as a result of removing causation: Spurious (nonsense) correlations
- Resulting from e.g. [[Confounding Variable]]s, [[Simpson's Paradox]], 

**So the chapter is essentially the history of how causality was removed from statistics**.

The chapter then talks about Sewall Wright and his use of path diagrams (see [[Path Analysis]]), which basically brought causation a bit back into the field. These diagrams also include a [[Path Coefficient]].

It goes on to talk about how Wright's idea was continuously brought down and challenged, but later resurfaced. Path analysis was taken and turned to [[Structural Equation Modeling (SEM)]] - but some said SEM has nothing to do with [[Causation]]. 

The chapter also shortly introduces [[Bayesian Analysis]], but say that even this still doesn't fully introduce causation back to statistics. 

### Chapter 3
This chapter focuses on [[Bayesian Networks]], what they are, their current-day applications, and how they relate to [[Causation]].

It starts with some of the history of Thomas Bayes (whom the networks are named after), a Reverend and math enthusiast who pondered the question: *How much evidence would it take to convince us that something we consider improbable has actually happened? When does a hypothesis cross the line from impossibility to improbability and even to probability or virtual certainty?*

Bayes' paper showed that you can deduce the probability of a cause from an effect ([[Forward Probability]]). But his method ultimately was looking at how humans can assess [[Inverse Probability]]. 

The chapter goes on to talk more about Bayes and [[Inverse Probability]], linking it to [[Bayes' Rule]] and [[Bayesian Networks]]. 

The chapter then goes on to further explain [[Bayesian Networks]] through their relation to [[Artificial Intelligence]] and [[Neural Networks]]. Basically going a bit over a simplified version of AI history: 
*Simplified history of AI*
1. Looking at Expert systems to create AI
2. Probability for AI --> leading to Bayesian networks etc.
3. Causality for AI

They then go on to explain how the links (junctions) between different nodes in the network have three basic types (when dealing with a three-node network)
1. Chain
2. Fork
3. Collider
(See [[D-Separation]])

[[Conditional Probability Table]] is then brought up to showcase how the different nodes "listen" to each other. 

The chapter then goes on a bit about how Bayesian networks are used today, e.g. for phones, victim identification etc.

Finally, the chapter sets Bayesian networks a bit in relation to causal diagrams - basically saying that Bayesian Networks are the lowest rung of the [[Ladder of Causality]], and causal networks are higher steps.

### Chapter 4
This chapter starts with a short history introduction to the concepts of an [[Experiment]] and [[Experimentation]]. It then highlights the importance of understanding [[Confounding Variable]]s and how to deal with them (see [[Confounding]]), as well as list them as a possible [[Bias]]. 

The chapter states that [[Confounding]] is a causal concept—it belongs on rung two of the [[Ladder of Causality]], and 

The chapter then goes on to explain the history of [[Randomized Controlled Trials (RCT)]], and how they relate to [[Causation]] and [[Confounding]]. 
- Basically talking about how randomization in [[Experiment]]s helps combat [[Confounding]]. 

The chapter then touches a bit more on the history of [[Confounding]] and how it hasn't really been clearly understood by statisticians for a long time. 

Finally, the chapter highlights the importance of the [[Do-operator]] and the [[Back-door Criterion]] for defining confounding, identifying confounders, and adjusting for them.
- Basically saying we shouldn't always control for everything. We need to use [[Causal Diagram]]s and understand the types listed in [[D-Separation]]. 

### Chapter 5
The chapter starts out with looking back at the debate surrounding the relationship between smoking and lung cancer. Basically telling how some argued that smoking and lung cancer were correlated due to a "lurking third variable" ([[Confounders]]), while other said it was a cause. 

It goes on to tell more about the smoking debate, and leads into explaining how sometimes [[Randomized Controlled Trials (RCT)]] are simply not possible to conduct - which is why we need other ways to determine causality.

It says case-control studies were conducted, but these had with them all sorts of various [[Bias]]. This therefore let to a questionnaire about smoking habits which provided new results. However, there was still arguments such as *"They (smokers) may be genetically or “constitutionally” different from nonsmokers in a number of ways—more risk taking, likelier to drink heavily"*.

They then end up with [[Hill´s Criteria]]/viewpoints, but also state that they may be lacking in some areas.

The chapter then tells about the correlation between smoking mothers and low birth weight and mortality of their babies. This section highlights the importance of understanding colliders (see [[Structural Causal Models]] and [[Collider Bias]]), as, e.g:
*"If we find out that the mother is a smoker, this explains away the low weight and consequently reduces the likelihood of a serious birth defect. But if the mother does not smoke, we have stronger evidence that the cause of the low birth weight is a birth defect, and the baby’s prognosis becomes worse."*

![[Pasted image 20230710210343.png]]

The collider is Birth Weight. By looking only at babies with low birth weight, we are conditioning on that collider

### Chapter 6
This chapter states that it will focus on paradoxes within the field of statistics, such as the [[Simpson's Paradox]] and [[Monty Hall Problem]], and view them with a more "causal lens".

The chapter goes on to discuss the [[Monty Hall Problem]] in more detail, highlighting the importance of understanding both the data and the data-generating process (how the the data is obtained). The problem is used to explain how our brains are not wired to do probability problems, but they are wired to do causal problems.

