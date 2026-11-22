---
title: Procedure
template: default

---

1. Center the data by subtracting the mean of each feature.
2. Store the means of each feature in a vector $\mu$ for later use in reconstructing the data.
3. Compute the covariance matrix of the centered data.
4. Compute the eigenvalues and eigenvectors of the covariance matrix.
5. Sort the eigenvalues in descending order and select the top $k$ eigenvectors corresponding to the largest eigenvalues. These eigenvectors form the principal components.
6. Compute the component scores $Z=XW$ by projecting the centered data onto the selected principal components. The component scores represent the data in the new feature space defined by the principal components.


To reconstruct data from the principal components, we can use the following formula:
$$
X_{reconstructed} = Z W^T + \mu
$$
Where $Z$ is the matrix of component scores, $W$ is the matrix of selected eigenvectors (principal components), and $\mu$ is the mean of the original data. This allows us to approximate the original data using a reduced number of features while preserving as much variance as possible.   

