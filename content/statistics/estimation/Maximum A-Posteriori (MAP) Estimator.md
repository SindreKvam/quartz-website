The MAP estimator is very similar to the [[Maximum Likelihood Estimation (MLE)|MLE]]. The difference is that we use a-posteriori information using Bayes theorem.
$$
\hat\theta_{MAP} = \arg\max_\theta p(\theta|x)=\arg\max_\theta p(x|\theta)p(\theta)
$$
From Bayes theorem, a $p(x)$ is missing, but this does not affect the peak of the PDF, meaning that it is not needed here.