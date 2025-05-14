
The maximum a-posteriori classifier, also named the *Bayes Decision Rule* (BDR) is given by:
$$
x\in\omega_j \Leftrightarrow P(\omega_j|x)=\max_iP(\omega_i|x)
$$
which, by applying Bayes law can be written as:
$$
\hat\omega=\arg\max_{\omega_i}p(x|\omega_i)P(\omega_i)
$$
**Note**:
- The BDR/MAP classifier is only a theoretically optimal classifier. The densities and probabilities are never known exactly.
- One will have to choose a parametic form (for example Gaussian), and then estimate the parameters that fits for the chosen parametic.
___
## The Plug-in MAP classifier
The most common parametic form is the Gaussian density:
$$
p(x|\omega_i)=\mathcal{N}\left(\mu_i, \Sigma_i\right)=\frac{1}{\sqrt{(2\pi)^L}\det({\boldsymbol{C}})}\exp\left(-\frac{1}{2}(\boldsymbol{x}-\mu_i)^T\boldsymbol{C}^{-1}_i(\boldsymbol{x}-\mu_i)\right)\quad i=1,2,...,C
$$
Where $L$ is the *input feature* dimension.

This can further be described in terms of *discriminants*.
$$
\hat\omega=\arg\max_i\left( -\frac{L}{2}\log(2\pi)-\log(\det{C})-\frac{1}{2}(x-\mu_i)^TC^{-1}(x-\mu_i) \right)
$$

$$
\begin{aligned}
g_i(x)&=-\frac{L}{2}\log(2\pi)-\log(\det{C})-\frac{1}{2}(x-\mu_i)^TC^{-1}(x-\mu_i)\\
&=\frac{1}{2}x^TC^{-1}x +\mu_i^TC^{-1}x- \frac{1}{2}\mu_i^TC^{-1}\mu_i -\frac{L}{2}\log(2\pi)-\log(\det{C})\\
&=\mu_i^TC^{-1}x- \frac{1}{2}\mu_i^TC^{-1}\mu_i + K
\end{aligned}
$$
where $K=\frac{1}{2}x^TC^{-1}x-\frac{L}{2}\log(2\pi)-\log(\det{C})$.

By plugging in values for $\mu_i$ and $C^{-1}$ we can find the discriminants $\boldsymbol{g}=(g_0,g_1,...,g_L)^T$.
To find the separation lines, go through all discriminants and set them equal each others.
$$
g_j(x)=g_i(x)\quad \forall i\neq j
$$
