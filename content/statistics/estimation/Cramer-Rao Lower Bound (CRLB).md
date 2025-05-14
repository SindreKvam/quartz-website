---
tags:
  - estimation
  - statistics
---

## Definition
The variance of any unbiased estimator $\hat\theta$ must satisfy:

$$
\mathrm{Var}(\hat\theta) \ge \frac{1}{-E\left[\frac{\partial^2}{\partial\theta^2} \ln p(\mathbf{x};\theta) \right]}
$$

An unbiased estimator may be found that attains the bound for all $\theta$ if and only if we can write the regularity condition in the specific form.
___
## Special Form
If we are able to write the regularity conditions in the following specific form:

$$
\frac{\partial}{\partial\theta}\ln p(\mathbf{x};\theta) = I(\theta)\left(g(\mathbf{x}) - \theta\right)
$$

Then we have found the [[Minimum-Variance Unbiased (MVU) Estimator|MVU]] estimator; $\hat\theta=g(\mathbf{x})$, and the minimum variance is given by $\mathrm{Var(\hat\theta)}\ge 1/I(\theta)$

If we are not able to write the regularity condition in the specific form, there exists no [[Minimum-Variance Unbiased (MVU) Estimator|MVU]] estimator. If this is the case, the CRLB can still, in most cases, be determined so that it can be used to compare the performance of the estimator to the minimum possible variance.