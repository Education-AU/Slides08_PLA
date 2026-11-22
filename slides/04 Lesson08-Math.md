---
title: The Math
template: default

---

The first condition is that the data is centered.

The data is represented by the matrix $X$ of size $m \times n$, where $m$ is the number of samples and $n$ is the number of features. The data is centered if the mean of each feature is zero, which can be expressed mathematically as:
$$
\frac{1}{m} \sum_{i=1}^{m} X_{ij} = 0 \quad \text{for all } j = 1, 2, \dots, n.
$$  
This is obtained by subtracting the mean of each feature from the data.

The second condition is that the directions in which the data is represented are orthogonal