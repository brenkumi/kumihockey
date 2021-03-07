---
title: "CMSAC '20: Clustering and Analyzing 5v5 NHL Shot Location Data"
summary: "My poster presenting my work on clustering 5v5 NHL shot maps at the 2020 Carnegie Mellon Sports Analytics Conference poster competition. I find 10 clusters of players based off of their shooting patterns and analyzing the composition of these clusters."
diagram: yes
date: '2020-10-25'
markup: mmark
math: yes
image:
  caption: null
  placement: null
links:
- icon: file-pdf
  icon_pack: fas
  name: Poster
  url: https://www.dropbox.com/s/f79tyyyflhgtd1h/CMSAC%20-%20Clustering%20and%20Analyzing%205v5%20NHL%20Shot%20Location%20Data.pdf?dl=0
- icon: black-tie
  icon_pack: fab
  name: Conference Webpage
  url: http://www.stat.cmu.edu/cmsac/conference/2020/
- icon: r-project
  icon_pack: fab
  name: Data and R Code
  url: https://www.dropbox.com/s/320c6amwyirarbw/NHL-5v5-Shot-Clustering-Project.zip?dl=0
---

I presented my work on clustering NHL player 5v5 shot heatmaps at the Carnegie Mellon Sports Analytics Conference poster competition.

### Abstract

Heatmap-style visualizations are a popular and intuitive way to display shot location data in hockey. However, these visualizations do not allow for large scale player comparison. In this poster, I provide a solution to this issue by clustering NHL players based on their even strength shot locations over three seasons (2017-18 to 2019-20) and analyzing the results.

The clustering consists of two stages. First, I fit a 565 square shot density polygrid to each player’s shot locations through the use of 2D-Gaussian kernel density estimation. Following that, I perform Ward's linkage hierarchical clustering to group players based on their shot polygrids. 

This methodology results in 10 clusters that can be broken down into three subgroups: home plate forwards, perimeter forwards and defencemen. Upon forming these clusters, I analyze the results through comparing overall shot heatmaps, the top scorers, and the distribution of expected unblocked shooting percentage, actual unblocked shooting percentage, and player height for each cluster.
