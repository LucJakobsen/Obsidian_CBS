Naive Bayes is [[Supervised Learning]] algorithm based on applying [[Bayes' Rule]] with the naive assumption of conditional independencies between every pair of [[Variable]]s/features given the class in the response variable ([[Dependent Variable]]).



In Python, to use the Naive Bayes that can deal with both numerical and categorical variables, you need to install and use mixed-naive-bayes:
``pip install mixed-naive-bayes``
``from mixed_naive_bayes import MixedNB``


### Pros and Cons of Naive Bayes
**Pros:**
- Very simple, easy to understand
- Fast and efficient
- Perform well for small datasets or simple tasks

**Cons**
- Naive assumptions may not valid empirically
- Performance is generally not as good as other sophisticated models such ANNs or tree-based models

