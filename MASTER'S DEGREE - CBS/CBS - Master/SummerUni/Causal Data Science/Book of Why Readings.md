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

Galton continues his research on linkage between father and son genetics (e.g. height), leading to the [[CBS - Master/1st Semester/Understanding and Regulating Data-driven Business Models/Regression|Regression]] line and the finding that correlation does not mean causation. Later his disciple, Karl Pearson, created the correlation coefficient.

So basically, Galton proved that regression to the mean does not require a causal explanation, and Pearson then took this and said "causality isn't needed and it can't be proved".

But Pearson discovered quite a few problems as a result of removing causation: Spurious (nonsense) correlations
- Resulting from e.g. [[Confounding Variable]]s, [[Simpson's Paradox]], 

**So the chapter is essentially the history of how causality was removed from statistics**.

The chapter then talks about Sewall Wright and his use of path diagrams (see [[Path Analysis]]), which basically brought causation a bit back into the field. These diagrams also include a [[Path Coefficient]].

It goes on to talk about how Wright's idea was continuously brought down and challenged, but later resurfaced. Path analysis was taken and turned to [[Structural Equation Modeling (SEM)]] - but some said SEM has nothing to do with [[Causation]]. 

The chapter also shortly introduces [[Bayesian Analysis]], but say that even this still doesn't fully introduce causation back to statistics. 



