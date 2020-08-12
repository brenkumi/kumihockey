---
title: "Categorizing OHL PP Styles Using Hierarchical Clustering"
summary: "In this article I will demonstrate how to group players based on their power play shot charts through Ward's Linkage Hierarchical Clustering. Following that I will use bootstrap resampling to generate confidence intervals for each player"
diagram: yes
date: '2020-07-25'
markup: mmark
math: yes
image:
  caption: null
  placement: null
---








# Introduction

If you are a follower of hockey analytics, you've probably heard the term clustering before. If you haven't, clustering is a machine learning method that groups together similar observations in our data.

There has been some great work applying clustering to hockey in the past including the clustering of pass locations by David Yu and the SportLogiq team at [CBJHAC](https://www.youtube.com/watch?v=TENd93QJt-8&t=6852s) and [ISOLHAC](https://www.youtube.com/watch?v=Q-kWb6Vshmo&t=1860s) as well as Daniel Weinberger on [HockeyGraphs](https://hockey-graphs.com/2019/09/04/visualizing-and-quantifying-passing-on-the-power-play/) and the clustering of player activity by Schulte et al. at [SSAC 2017](https://www.cs.sfu.ca/~oschulte/files/pubs/sloan-fix.pdf) just to name a couple and I hope to build on that by using **hierarchical clustering to group OHL players based on their power play shooting patterns**.

The motivation behind this project is to gain an understanding of where OHL players are positioned on the power play and how this may affect their goal/point totals for casual fans who may not be able to watch OHL games on a regular basis and also to identify and analyze any interesting cases that appear in the clusters.

The data is my cleaned up version of the OHL play-by-play data, which was scraped and shared by Dave MacPherson on [Twitter](https://twitter.com/davemacp/status/1239306719253204994). This pbp data did not include the strength state of each shot, it just had shot and penalty times, so I did what I could to classify the strength states, however, there is likely a slight margin of error of roughly +/- 5 shots for each player.




Shot Charts

# What is Hierarchical Clustering?

As mentioned in the introduction, clustering is a machine learning method used to group together similar observations in our data. In this article, I will be using Ward's Linkage Agglomerative Hierarchical Clustering to group players with at least 40 PP shots on goal based on where their shots are coming from. 

**Agglomerative hierarchical clustering** is a simple algorithm for grouping players and is commonly referred to as the "bottom-up" approach. We begin with all players in their own cluster, then we repeatedly combine the two most similar clusters together over and over until we have one big cluster. Following the creation of the tree diagram (called a dendrogram), we can "cut the tree" when we reach the desired number of clusters. This process is demonstrated in the video below. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/phtVghlqXT8" frameborder="0" allowfullscreen></iframe>

**Ward's linkage** refers to criteria we use to measure distance between clusters. In Ward's linkage, we merge the two clusters that result in the smallest increase in overall deviation from the cluster centre. 

For more information on hierarchical clustering, [this video](https://www.youtube.com/watch?v=7xHsRkOdVwo) provides a good introduction and [this video](https://www.youtube.com/watch?v=vg1w5ZUF5lA) provides a further explanation of linkages.

## Why Use Hierarchical Clustering?



Pros and cons

Why it is good for us

# Preparing the Data

Why we need to bin the data

How we bin it (diagram)

# Clustering Results

Dendrogram

## Cluster 1

## Cluster 2

## Cluster 3

## Cluster 4

## Cluster 5

# Interesting Observations

## The Sudbury 1-1-3

Byfield-Loponen-Thompson

## The OHL's Dustin Byfuglien

Regula

## The 5 Man PP

NB Struthers

## The Issues

Rossi & Wright

# Bootstrapping

Sam's article

Motivation: Rossi, Wright; find players like these

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




