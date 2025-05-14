---
title:
---

The BLUE is another unbiased estimator. The BLUE restricts the estimator to be linear in the data;
$$
\hat\theta = \sum^{N-1}_{n=0} a_nx[n].
$$
To find the BLUE we use the constraint that comes with an unbiased estimator.
$$
E(\hat\theta) = \sum^{N-1}_{n=0} a_nE(x[n])=\theta
$$
It can be found that the variance of $\hat\theta$ is given by $\mathrm{Var}(\hat\theta)=\boldsymbol{a}^T\boldsymbol{Ca}$. To find the best estimator, we need to minimize the variance.

The BLUE estimator is in the end found to be given as
$$
\hat\theta=\frac{\boldsymbol{s}^T\boldsymbol{C}^{-1}\boldsymbol{x}}{\boldsymbol{s}^T\boldsymbol{C}^{-1}\boldsymbol{s}}
$$
Where $\boldsymbol{s}$ is the scaled mean; $E(x[n])=s[n]\theta$. As we assume that the mean of $x[n]$ is linear in $\theta$. And $\boldsymbol{C}$ is the covariance matrix.
___
## BLUE on Vector Form
The BLUE on vector form can be shown to be given as
$$
\boldsymbol{\hat\theta}= (\boldsymbol{H}^T\boldsymbol{C}^{-1}\boldsymbol{H})^{-1}\boldsymbol{H}^T\boldsymbol{C}^{-1}\boldsymbol{x}
$$
___
## Properties
- If $\hat{\theta}_{BLUE} = \hat{\theta}_{ML}$, then the estimator is the MVU estimator.