
## Motivation
In electronic systems, we often design systems to extract information. Whichever way you do this, you have to estimate values of a group of parameters.

These parameters can be anything from the DC-level from a voltage source with a lot of noise present to estimating the distance a radar signal travels before hitting an object and bouncing back.
___
## Terminology:
- ***Effective estimator***: An estimator is effective if it reaches the minimum variance possible given by the [[Cramer-Rao Lower Bound (CRLB)|Cramer-Rao lower bound]].
- ***Unbiased estimator***: An estimator where the estimated value is the value we want to estimate; $E(\hat\theta)=\theta$.
___
## Models
- [[Cramer-Rao Lower Bound (CRLB)]]
- [[Linear Models]]
___
## Estimation Methods
There are a few estimation methods available, the most common are listed here, starting with the most accurate.
- [[Minimum-Variance Unbiased (MVU) Estimator]]
- [[Best Linear Unbiased Estimators (BLUE)]]
- [[Maximum Likelihood Estimation (MLE)]]
___
## Bayesian Estimation Methods
- [[Minimum Mean Square Error (MMSE) Estimator]]
- [[Maximum A-Posteriori (MAP) Estimator]]
