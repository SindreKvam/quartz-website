---
tags:
  - statistics
  - estimation
date: 2025-05-14
description:
---
The minimum variance unbiased estimator is the best possible estimator that can be designed.
The MVU estimator does not, in general, exist. But when they do, the methods of finding the MVU rely on the [[Cramer-Rao Lower Bound (CRLB)|Cramer-Rao lower bound]].

If the MVU does not exist, further constraints on the estimator has to be added, which leads to alternative, but suboptimal estimators.
___
## Unbiased
An estimator is *unbiased* if:

$$
E(\hat\theta) = \theta \quad,\quad a<\theta<b
$$

where $(a,b)$ denotes the range of possible values of $\theta$.
___
## Minimum-Variance
The minimum variance criteria cannot be defined to one specific criteria. One natural optimality criteria is the *mean square error* (MSE) that is defined as:

$$
\mathrm{mse}(\hat\theta) = E\left[ (\hat\theta-\theta)^2 \right]
$$
