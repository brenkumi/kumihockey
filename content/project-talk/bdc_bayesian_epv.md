---
title: "BDC '21: Bayesian Space-Time Models for Expected Possession Added Value"
summary: "A group submission for the Stathletes' Big Data Cup 2021 along with Tyrel Stokes, Mikael Nahabedian, and Thibaud Châtel. Our work involved quantifying the value of each event in offensive entry-to-exit sequences using a Markov decision process with transition probabilities estimated via INLA."
diagram: yes
date: '2021-03-05'
markup: mmark
math: yes
image:
  caption: null
  placement: null
links:
- icon: file-pdf
  icon_pack: fas
  name: Paper
  url: https://github.com/brenkumi/BigDataCup2021/blob/main/Final%20Paper/BDC21%20-%20Bayesian%20Space-Time%20Models%20for%20Expected%20Possession%20added%20Value.pdf
- icon: r-project
  icon_pack: fab
  name: Data and Code
  url: https://github.com/brenkumi/BigDataCup2021
---

To date, public hockey analysis has largely been limited to shot data and manually-tracked microstats. I had the pleasure of working with the brilliant minds of Tyrel Stokes, Mikael Nahabedian and Thibaud Châtel to develop a comprehensive Bayesian Markov decision model that can estimate the value of each event in entry-to-exit play sequences. This model allows us to go beyond valuing events in isolation to capture the dependencies within the overall chain of events. Additionally, we use INLA (Integrated Nested Laplace Approximation) to estimate the fluid and dynamic spatiotemporal effects that evolve as a play develops. 

Using our model, we can run simulations to estimate the cumulative expected goals that will occur from the rest of the sequence beyond the current play. This idea is borrow largely from [Cervone et al.](https://www.tandfonline.com/doi/abs/10.1080/01621459.2016.1141685?journalCode=uasa20)'s "Expected Possession Value" (EPV or xPV). By taking the increase/decrease in xPV between an event and the subsequent event, we estimate a metric we call the "Possession Added Value" (PAV); this metric can be interpretted as the boost in expected goals due to the event. 

We also provide examples of how PAV can be used in scouting at both the team and player-level.

Our dataset consisted of 40 Erie Otters games from the 2019-20 OHL season that was graciously provided by Stathletes for this competition.



