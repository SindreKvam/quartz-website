
___
## Terminology
- ***Features***: explanatory variables: $x_l\quad l=1,2,...,L$.
- ***Feature vectors***: samples: $\boldsymbol{x}=(x_1,x_2,...,x_L)^T$
- ***Classes***: $\omega_m\quad m=1,2,...,M$
- ***Classifier***: partition of the feature space: $\Omega_m\quad m=1,2,...,M$
- ***Training pattern***: $\{x_n; \omega_{c(n)}\}$
- ***Training set***: $(\{x_1; \omega_{c(1)}\},\{x_2; \omega_{c(2)}\},...,\{x_N; \omega_{c(N)}\})$
___
## Formulas required to design classifiers
- ***A priori probabilities***: $p(\omega_i)\quad i=1,2,...,C$
- ***Class conditioned densities***: $p(x|\omega_i)\quad i=1,2,...,C$
- A posteriori probabilities: $p(\omega_i|x)\quad i=1,2,...,C$
- Joint distributions: $p(x,\omega_i)\quad i=1,2,...,C$ where:
	- $\sum_i p(x,\omega_i)=p(x)$ for any $x$
	- $\int p(x,\omega_i)dx=P(\omega_i) \quad i=1,2,...,C$
	- $p(x,\omega_i)=p(x|\omega_i)P(\omega_i)=P(\omega_i|x)p(x) \quad i=1,2,...,C$
