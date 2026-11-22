---
title: Motivation
template: default
---

We consider a large data set of points in a high-dimensional space.
This could be some measurements of height,weight,age, and other features of a population of people,which is represented
by a tall matrix where each row is a person and each column is a feature.

We want to find a low-dimensional representation of the data by creating fewer new features, each of which is a linear combination of the original features. 

The goal is to retain as much of the variance in the original data as possible. This is the purpose of Principal Component Analysis (PCA).

The new features (principal components) are chosen to maximize the variance of the data when projected onto these new
axes.
