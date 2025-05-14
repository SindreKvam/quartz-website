After defining the likelihood function $L(x)$ as stated by the [[Neyman-Pearson Theorem|Neyman-Pearson theorem]], we can find a test statistic $T(x)$.

After formulating
$$
L(x)=\frac{p(x;H_1)}{p(x;H_0)} \gt \gamma
$$
We can do some simplification, for example taking the logarithm, shifting values that do not change with $x$ over to the other side, we will end up with an equation on the following form:
$$
T(x)\gt f(\gamma) = \gamma^\prime
$$
By finding what type of distribution the test statistic is, the next step is to find the parameters in the different hypothesis cases. If the test statistic is Gaussian, we would find the mean and the variance.
$$
T(x)\sim \mathcal{N}(\mu_0, \sigma_0^2)\quad \text{under } H_0
$$
$$
T(x) \sim\mathcal{N}(\mu_1, \sigma_1^2)\quad \text{under } H_1
$$
The limits can now be written on the form of
$$
P_{FA}=p(T(x)\gt\gamma^\prime;H_0)\quad\text{and}\quad P_{D}=p(T(x)\gt\gamma^\prime;H_1)
$$
Which for the case for the Gaussian distribution can be normalized and re-written using the $Q$ function.
$$
P_{FA}=Q\left(\frac{\gamma^\prime-\mu_0}{\sqrt{\sigma_0^2}}\right)\quad\text{and}\quad P_D=Q\left(\frac{\gamma^\prime-\mu_1}{\sqrt{\sigma_1^2}}\right)
$$
These values can further be used to find the performance of the detector using [[Receiver Operating Characteristics (ROC)|ROC]].