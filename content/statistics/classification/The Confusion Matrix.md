The confusion matrix is a performance metric for classifiers.

| Event\\Decision    | $\boldsymbol{H}_0$ | $\boldsymbol{H}_1$     |
| ------------------ | ------------------ | ---------------------- |
| $\boldsymbol{H}_0$ | $1-P_{FA}$ ()      | $P_{FA}$ (false alarm) |
| $\boldsymbol{H}_1$ | $1-P_D$ (miss)     | $P_D$ (detection)      |
___
## General Case

| Event\\Decision    | $\boldsymbol{H}_1$ | $\boldsymbol{H}_2$ | $\cdots$ | $\boldsymbol{H}_M$ |
| ------------------ | ------------------ | ------------------ | -------- | ------------------ |
| $\boldsymbol{H}_1$ | $A(1,1)$           | $A(1,2)$           |          | $A(1,M)$           |
| $\boldsymbol{H}_2$ | $A(2,1)$           | $A(2,2)$           |          | $A(2,M)$           |
| $\vdots$           |                    |                    | $A(i,j)$ |                    |
| $\boldsymbol{H}_M$ | $A(M,1)$           | $A(M,2)$           |          | $A(M,M)$           |

**Accuracy**: $Ac=\frac{1}{N}\sum^M_{i=1}A(i,i)$

The accuracy measures how often the models predictions are correct overall. Can be misleading if one class dominates, and drags the average up [[1]].

**Precision**: $P_j=\frac{A(j,j)}{\sum^M_{i=1}A(i,j)}$

The precision (vertical) measures the quality of the models positive predictions. How many of the instances predicted as positive are actually positive [[1]].

**Recall**: $R_i=\frac{A(i,i)}{\sum^M_{j=1}A(i,j)}$

The recall (horizontal) measures how well the model identifies all actual positive cases. It shows the proportion of true positives detected out of all the positive instances [[1]].


## References
[1]: https://www.geeksforgeeks.org/confusion-matrix-machine-learning/