---
title: "UCSAS: Point Trend Values II"
summary: "My poster presenting my updated work on Point Trend Values at the U-Conn Sports Analytics Symposium poster competition. This content is very similar to my presentation at ISOLHAC but with sounder methodology in the calculation of the metric and shared code and data. I finished the competition in a tie for 1st place with Nate Rowan."
diagram: yes
date: '2020-10-10'
markup: mmark
math: yes
image:
  caption: null
  placement: null
links:
- icon: file-pdf
  icon_pack: fas
  name: Slides
  url: https://www.dropbox.com/s/y13cgq5nro9yeg0/UCSAS%20-%20Point%20Trend%20Values%20II%20-%20Brendan%20Kumagai.pdf?dl=0
- icon: black-tie
  icon_pack: fab
  name: Poster Webpage
  url: https://statds.org/events/ucsas2020/poster_directory.html
- icon: r-project
  icon_pack: fab
  name: Data and R Code
  url: https://www.dropbox.com/s/x2dvbbitnpkbiy8/CHL-Trend-Values-Project.zip?dl=0
---

*Placement: Tie for 1st*

The general theory in hockey scouting is that if a player improves as the season goes on, then he or she can elevate to another level when the games become more meaningful and will be better able to adapt to professional hockey. In this poster, I put this idea to the test by taking game-by-game points data from OHL and WHL forwards between 2010-11 to 2018-19 and determining their "Point Trend Value" (PTV). A Point Trend Value is a new metric that I introduce here that measures a player's rate of improvement in cumulative point production over a season. 

After I define and calculate the Point Trend Value for each player, I determine that this metric has no influence on success beyond the current season but NHL teams still show some trends towards drafting prospects with increasing point production higher than others indicating some potential recency bias on the part of the teams.

There are a few minor differences in my methodology in this poster compared to my presentation at ISOLHAC:

1. Before fitting the quadratic regression model in the calculation of the metric, I 0-1 scaled each player's games played and cumulative points. Without scaling the data, the Point Trend Value tends to be exaggerated for players with lower games played or high point totals.

2. After fitting the quadratic model and taking the double derivative, I z-scored the data rather than multiplying it by 500. This has no effect on the results but z-scored values are easier to interpret for those with basic statistical knowledge.

3. In comparing how Point Trend Values affect draft results at a macro-level, I fit LOESS curves on a draft pick vs Pts/GP plot for three groups: upward trending (PTV > 1), steady (-1 < PTV < 1), and downward trending (PTV < -1). The results show that the upward trending group tends to have a lower Pts/GP at most points of the draft suggesting that teams may be slightly more forgiving of players with low Pts/GP if they finish off the season on a hot streak.
