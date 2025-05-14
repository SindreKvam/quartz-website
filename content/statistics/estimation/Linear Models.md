The linear model is a method of trying to solve a line-fitting problem. If we can assume that the system can be represented linearly, we should be able to create a model of our data:

$$
x[n]=A+Bn+w[n]\quad,\quad n=0,1,...,N-1
$$

In matrix notation we can make the model more compact.

$$
\mathbf{x}= \boldsymbol{H\theta} + \mathbf{w}
$$
where;

$$
\boldsymbol{x}=\left[x[0], x[1],...,x[N-1]\right]^T
$$
$$
\boldsymbol{w}=\left[w[0], w[1],...,w[N-1]\right]^T
$$
$$
\boldsymbol{\theta}=\left[A,B\right]^T
$$

Matrix $\boldsymbol{H}$ is referred to as the *observation matrix*.
___
## MVU Estimator
From the linear model, we can easily identify the [[Minimum-Variance Unbiased (MVU) Estimator|MVU]] estimator if it exists by attempting to find the *special form*.
___
### Example if the noise is Gaussian
By attempting to find the special form, we get:
$$
\frac{\partial\ln p(\boldsymbol{x};\boldsymbol{\theta})}{\partial\boldsymbol{\theta}} = \frac{\boldsymbol{H}^T\boldsymbol{H}}{\sigma^2}\left((\boldsymbol{H}^T\boldsymbol{H})^{-1}\boldsymbol{H}^T\boldsymbol{x}-\boldsymbol{\theta}\right)
$$
Which gives;
$$
\boldsymbol{\hat{\theta}} = (\boldsymbol{H}^T\boldsymbol{H})^{-1}\boldsymbol{H}^T\boldsymbol{x}
$$
$$
\boldsymbol{I}(\boldsymbol{\theta})=\frac{\boldsymbol{H}^T\boldsymbol{H}}{\sigma^2}
$$
And the covariance matrix, giving the minimum variance is given by $\boldsymbol{I}(\boldsymbol{\theta})^{-1}$.

___
## Best Linear Unbiased Estimators
From the linear model, we can easily identify the [[Best Linear Unbiased Estimators (BLUE)|BLUE]].