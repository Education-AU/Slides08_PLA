---
title: The Math
template: default

---


This is exactly the eigen-decomposition of the covariance matrix $X^TX$. The eigenvectors are the directions of the new features, and the eigenvalues are their variances. The new features are uncorrelated being orthogonal, and they capture the maximum variance in the data.

Now we can reduce the dimensionality of the data by keeping only the first $k$ features, which capture most of the variance in the data. This is done by selecting the first $k$ eigenvectors corresponding to the largest eigenvalues, and projecting the data onto this new subspace.

