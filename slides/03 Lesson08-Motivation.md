---
title: Motivation
template: two-column
showFooter : false
---

For example, the original 2D data points may cluster along a diagonal whose line of greatest spread does not pass through the origin:

```text
       y
       ↑       •
       |     •
       |   •    ↗ PC1
       | •    /
       |    /
       +--------------→ x
```
*Figure 1: Original data and its line of greatest spread.*

We can see that the data points are spread out along a line. In order two capture the data as a line we need to center the data by subtracting the mean of each feature. The centered points have their mean at the origin, and the PC1 direction now passes through the origin:


<!-- column -->

In a centered version the data looks like this:





```text
              y
              ↑       ↗ PC1
              |     •
              |   /
              | •
              |/
←-------------+-------------→ x
             /|
            • |
          /   |
        •     |
```

*Figure 2: The same data after centering, with PC1 through the origin.*

And now we can capture the data by a new feature (PC1) that is a linear combination of the original features. We can then represent each point by its position along PC1 instead of two coordinates, preserving most of the data's variation.