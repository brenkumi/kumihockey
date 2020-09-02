---
title: "Robustifying Cluster Results of OHL Player PP Shot Tendencies Using Bootstrapping"
summary: "In the first of two follow-up articles to my previous article on hierarchical clustering of OHL player PP shot tendencies, I will attempt to create bootstrap distributions of players' PP shot tendencies to give provide a closer look at which players fit in each cluster."
diagram: yes
date: '2020-08-25'
markup: mmark
math: yes
image:
  caption: null
  placement: null
---








# Introduction

Last article

Limitations and solutions: Rossi, Wright

Sam's article


# What is Bootstrapping?

Bootstrap distribution


# Bootstrap Results

Pros and cons

Why it is good for us


# Heatmaps?

# Conclusion




# The Code

## Loading and Preparing the Data

Load all necessary packages.

```
library(tidyverse)
```

Load the data set (this data can be found on my [Github](https://github.com/brenkumi/kumihockey) under content/article/projectdata).

```
ohl.shot.data = read_csv("projectdata/ohl-shot-data.csv")
```

## Creating Shot Maps of the Data


## Creating Regions and Binning the Data


## Performing Hierarchical Clustering


## Creating Heatmaps of the Data



## Bootstrapping the Data


## Confidence Intervals of Bootstrap Resampling




# References





