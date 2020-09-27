---
title: "Using Robust Sparse k-Means Clustering to Group NHL Players Based on ES Shot Locations (Not complete)"
summary: "In this article, I will build upon my work on clustering OHL PP shot data with a stronger approach. Using a larger sample size of three season of NHL even strength data, "
diagram: yes
date: '2020-10-05'
markup: mmark
math: yes
image:
  caption: null
  placement: null
---




# Introduction

# Hexbinning Approach

- Split F and D to improve the algorithm's ability to separate clusters

- Hexbin approach vs OHL PP approach (much smaller bins)

- Diagram of hexbins

- Concern: bins beside each other are treated no different from bins across ice

- Take delta of the mean for each bin


# Robust Sparse k-Means Clustering (RSKC)

- What is it?

- Why use it? (good for high-D data, downweights useless hexbins)

- Iterate 100x?

- Choosing k?


## RSKC Algorithm

- Explain the algorithm


# Clustering Results

- Visualization? Network?

# Interesting Observations

- TBD

# Conclusion

## Limitations


# The Code

# References





