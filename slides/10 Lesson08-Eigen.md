---
title: PCA using SVD
template: default

---
There are two common ways to compute PCA: using eigendecomposition (or SVD) of the covariance matrix, or using SVD directly on the centered data matrix. The latter is generally more numerically stable and is preferred in practice.

### 1. SVD of the covariance matrix

- Compute the covariance matrix of the centered data and perform eigendecomposition (or SVD) on it. The eigenvectors of the covariance matrix are the principal-component directions, and the eigenvalues give the variance explained by each component.
- Since the covariance matrix is symmetric and positive semidefinite, its left and right singular vectors can be chosen to be equal (up to sign choices). Thus, in its SVD, \(U=V\).
- The component scores are \(Z=XV\).
- The reconstruction of the centered data is \(X=ZV^T\), when all components are retained. With only \(k\) components, \(X_k=Z_kV_k^T\).
