---
title: The Math
template: default
showFooter: false

---
But we want many such **orthonormal** weights so we rewrite in matrix form, where $W$ is a matrix of size $n \times n$
whose columns are the weights for each new feature:
$$
\Lambda = W^TX^TXW(W^TW)^{-1}
$$

Where the condition is that the new features are orthonormal, which means that $W^TW = I$.

So
$$
\Lambda = W^TX^TXW
$$
Where $\frac{1}{m-1}X^TX$ is the covariance matrix of the data, and $\Lambda$ is a diagonal matrix whose entries are the
variances of the new features. We do not at this stage need the scaling factor $\frac{1}{m-1}$, so we will ignore it in
the following.