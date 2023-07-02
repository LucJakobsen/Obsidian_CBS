Bayes' Rule (or theorem) is a fundamental principle within probability and statistics. It relies upon the concept of [[Conditional Probability]]. 

It solves the problem of [[Inverse Probability]], and is a key part of [[Bayesian Networks]]. 
- Here's how: *we can estimate the conditional probability directly in one direction, for which our judgment is more reliable, and use mathematics to derive the conditional probability in the other direction, for which our judgment is rather hazy*

This is also what it does for [[Bayesian Networks]]:
- We tell the computer the [[Forward Probability]], and the computer tells us the inverse probabilities when needed


In its basic form, Bayes' rule is represented as:

P(A|B) = P(B|A) * P(A) / P(B)

- P(A|B): The conditional probability of event A given event B, also known as the posterior probability. This is what we aim to find using Bayes' rule.
	- *I.e. the probability of B given that A has occurred*
    
- P(B|A): The conditional probability of event B given that event A has already occurred.
    
- P(A) and P(B): The probabilities of A and B independently occurring, often referred to as the prior probabilities.


A large part of human belief about future events rests on the frequency with which they or similar events have occurred in the past. Bayes’s rule lets us attach numbers to this reasoning process.