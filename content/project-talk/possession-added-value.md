---
title: "Bayesian Space-Time Models for Expected Possession Added Value"
summary: "This project was joint work along with Tyrel Stokes, Mikael Nahabedian, and Thibaud Châtel for the 2021 Stathletes' Big Data Cup. Our work involved quantifying the value of each event in offensive entry-to-exit sequences through the use of various Bayesian spatiotemporal models and a Markov Decision Process. Our team was awarded 1st place out of 71 submissions."
diagram: yes
date: '2021-03-26'
markup: mmark
math: yes
image:
  caption: null
  focal_point: null
links:
- icon: file-pdf
  icon_pack: fas
  name: BDC Paper
  url: https://github.com/brenkumi/BigDataCup2021/blob/main/Final%20Paper/BDC21%20-%20Bayesian%20Space-Time%20Models%20for%20Expected%20Possession%20added%20Value.pdf
- icon: file-pdf
  icon_pack: fas
  name: BDC Slides
  url: https://www.dropbox.com/s/6z66zdy6o9qzr6y/BDC%20-%20Bayesian%20Space-Time%20Models%20for%20Expected%20Possesion%20Added%20Value.pdf?dl=0
- icon: youtube
  icon_pack: fab
  name: BDC Presentation
  url: https://www.youtube.com/watch?v=etTYTFt4Z-Y&t=2260s
- icon: github
  icon_pack: fab
  name: Data and Code
  url: https://github.com/brenkumi/BigDataCup2021
- icon: book-open
  icon_pack: fas
  name: Hockey Graphs Article I
  url: https://hockey-graphs.com/2021/07/06/bayesian-space-time-models-for-expected-possession-added-value-part-1-of-2/
- icon: book-open
  icon_pack: fas
  name: Hockey Graphs Article II
  url: https://hockey-graphs.com/2021/08/09/bayesian-space-time-models-for-expected-possession-added-value-part-2-of-2/
- icon: podcast
  icon_pack: fas
  name: Hockey IQ Podcast
  url: https://podcasts.apple.com/il/podcast/kumagai-nahabedian-ch%C3%A2tel-stokes/id1524738355?i=1000536956909
- icon: youtube
  icon_pack: fab
  name: SFU SAG Presentation
  url: https://www.youtube.com/watch?v=WkT5MpoxhQI
---

*Placement: 1st out of 71*

To date, public hockey analysis has largely been limited to shot data and manually-tracked microstats. I had the pleasure of working with the brilliant minds of Tyrel Stokes, Mikael Nahabedian and Thibaud Châtel to develop a comprehensive Bayesian Markov decision model that can estimate the value of each event in entry-to-exit play sequences. This model allows us to go beyond valuing events in isolation to capture the dependencies within the overall chain of events. Additionally, we use INLA (Integrated Nested Laplace Approximation) to estimate the fluid and dynamic spatiotemporal effects that evolve as a play develops. 

Using our model, we can run simulations to estimate the cumulative expected goals that will occur from the rest of the sequence beyond the current play. This idea is borrow largely from [Cervone et al.](https://www.tandfonline.com/doi/abs/10.1080/01621459.2016.1141685?journalCode=uasa20)'s "Expected Possession Value" (EPV or xPV). By taking the increase/decrease in xPV between an event and the subsequent event, we estimate a metric we call the "Possession Added Value" (PAV); this metric can be interpretted as the boost in expected goals due to the event. 

We also provide examples of how PAV can be used in scouting at both the team and player-level.

Our dataset consisted of 40 Erie Otters games from the 2019-20 OHL season that was graciously provided by Stathletes for this competition.



