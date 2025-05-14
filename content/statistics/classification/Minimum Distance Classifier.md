___
## Euclidian Distance
Euclidian distances are used when the covariance matrix is given by $\boldsymbol{C}_i=\sigma^2\boldsymbol{I} \quad \forall i$.
$$
d^2_E(\boldsymbol{x}_1,\boldsymbol{x}_2) = (\boldsymbol{x}_1-\boldsymbol{x}_2)^T (\boldsymbol{x}_1-\boldsymbol{x}_2) = ||\boldsymbol{x}_1-\boldsymbol{x}_2||^2
$$

___
## Mahalanobis Distance
Mahalanobis distance is used when covariance matrix is given by $\boldsymbol{C}_i = C \quad \forall i$.
$$
d^2_M(\boldsymbol{x}_1,\boldsymbol{x}_2) = (\boldsymbol{x}_1-\boldsymbol{x}_2)^T \boldsymbol{C}^{-1}(\boldsymbol{x}_1-\boldsymbol{x}_2)
$$
___
## K-means Clustering
We want to minimize
$$
J=\sum_{n=0}^N\sum_{k=0}^K r_{n,k}||\boldsymbol{x}_n-\boldsymbol{\mu}_k||^2
$$
Where if $\boldsymbol{x}_n$ belongs to cluster $k$, the indicators are as folllows:
$$
r_{n,j}=1,\quad j=k \quad\text{and}\quad r_{n,j}=0,\quad j\neq k
$$
We want to solve the optimation problem
$$
\arg\min_{\{r_{n,k}\}\{\boldsymbol{\mu}_k\}} J
$$

The solution to this is easily done iteratively.
- Choose arbitrary initial centers: $\{\boldsymbol{\mu}_1(0),...,\boldsymbol{\mu}_K(0)\}$.
- For each sample $\boldsymbol{x}_n$:
	- Identify the closes centre.
	- set the corresponding indicator accordingly.
- For each cluster:
	- Compute the barycenter for the samples that correspond to the cluster.
	- Update the new set of centers $\{\boldsymbol{\mu}_1(t+1),...,\boldsymbol{\mu}_K(t+1)\}$.

___
## Gaussian Mixtures (GMs)
...