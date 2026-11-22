---
title: PCA using SVD
template: default

---

### 2. SVD of the data matrix

- Perform SVD directly on the centered data matrix, with data points as rows and features as columns:
  \[
  X=U\Sigma V^T
  \]
  The right singular vectors (columns of \(V\)) give the principal-component directions.
- The variance explained by component \(i\) is:
  \[
  \lambda_i=\frac{\sigma_i^2}{m-1}
  \]
  where \(\sigma_i\) is its singular value and \(m\) is the number of data points.
- The component scores are \(Z=U\Sigma\).
- The reconstruction of the centered data is \(X=ZV^T\), when all components are retained. With only \(k\) components, \(X_k=Z_kV_k^T\).
