
The maximum a-posteriori classifier, also named the *Bayes Decision Rule* (BDR) is given by:
$$
x\in\omega_j \Leftrightarrow P(\omega_j|x)=\max_iP(\omega_i|x)
$$
which, by applying Bayes law can be written as:
$$
x\in\omega_j \Leftrightarrow p(x|\omega_j)P(\omega_j)=\max_ip(x|\omega_i)P(\omega_i)
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
Where $D$ is the *input feature* dimension.
