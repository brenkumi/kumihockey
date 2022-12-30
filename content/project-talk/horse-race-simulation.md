---
title: "Bayesian Velocity Models for Horse Race Simulation"
summary: "This project was joint work with Tyrel Stokes, Kimberly Kroetch, Gurashish Bagga, and Liam Welsh for the 2022 NYRA/NYTHA Big Data Derby competition. We leverage the horse racing tracking data provided in the competition to develop Bayesian B-spline regression models to forecast the probability that each horse will finish in each possible finishing placement. Our team was awarded 1st place out of 108 submissions."
diagram: yes
date: '2022-11-10'
markup: mmark
math: yes
image:
  caption: null
  focal_point: null
links:
- icon: kaggle
  icon_pack: fab
  name: Kaggle Submission
  url: https://www.kaggle.com/code/bkumagai/bayesian-velocity-models-for-horse-race-simulation
- icon: github
  icon_pack: fab
  name: Data and Code
  url: https://github.com/brenkumi/canadian-pharoah
---

*Placement: 1st out of 108*

The 2022 Big Data Derby, organized by the NYRA and NYTHA, provided data scientists with a previously untouched source of horse racing tracking data.

In Tyrel Stokes, Kimberly Kroetch, Gurashish Bagga, Liam Welsh, and I's submission for the Big Data Derby, we focused on developing a model to predict the probability that any given horse will finish in any possible place (i.e., 1st, 2nd, 3rd, etc.) dynamically at any point in the race. To do so, we developed Bayesian B-spline models to predict the forward and lateral velocity of each horse and used these models to simulate forward a race from any given situation.

Our Kaggle submission linked above describes our approach in further detail.

