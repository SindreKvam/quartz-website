The Neyman-Pearson Theorem states that to maximize $P_D$ for a given $P_{FA} = \alpha$ decide $H_1$ if 
$$
L(x)=\frac{p(x;H_1)}{p(x;H_0)} \gt \gamma
$$
Where the threshold $\gamma$ is found from
$$
P_{FA}=\int_{\{x:L(x)>\gamma\}}p(x;H_0)dx = \alpha
$$
The value $L(x)$ is named the likelihood ratio, and the test is named the *likelihood ratio test* (LRT).

There does also exist a *generalized likelihood ratio test* (GLRT).
$$
L_G(x)=\frac{p(x;\boldsymbol{\hat\theta}_1,H_1)}{p(x;\boldsymbol{\hat\theta}_0,H_0)} \gt \gamma
$$
where $\boldsymbol{\hat\theta}_l$ is the [[Maximum Likelihood Estimation (MLE)|MLE]] of $\boldsymbol{\theta}_l$.