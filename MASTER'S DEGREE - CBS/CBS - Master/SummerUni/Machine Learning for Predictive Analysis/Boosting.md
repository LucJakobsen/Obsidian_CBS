**Boosting** is sequential [[Ensemble Learning]] method where the base learners are generated sequentially. The basic motivation of sequential methods is to exploit the dependence between the base learners, since the overall performance can be boosted in a residual-decreasing way.

In theory, boosting methods are slightly better than bagging methods mainly because base learners improve over the iterations. However, this is not always true in practice. From another aspect, training bagging methods can be faster than boosting methods.

Two examples of boosting algorithms are:
1. [[AdaBoost]]
2. [[Gradient Boosting]]