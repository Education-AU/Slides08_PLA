---
title: The Math
template: default
showFooter: false

---

Now we have the matrix $X$ of size $m \times n$, where $m$ is the number of samples and $n$ is the number of features.

The data is centered if the mean of each feature is zero.

In order to understand the procedure we first look at the construction of at one new feature, the first principal
component. The first principal component is a linear combination of the original features, and it is the direction in
which the data varies the most.

That is we want to maximize the projection of each data point onto a direction $w$ of unit length:
$$
\lambda_1 =  ||X\frac{w}{||w||}||^2= \frac{||Xw||^2}{||w||^2} = \frac{w^TX^TXw}{w^Tw}
$$
