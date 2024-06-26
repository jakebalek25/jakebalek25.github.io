---
title: "Has Cleveland Created A 'Wind-Powered' Long Ball Haven With Their Recent Stadium Renovations?"
date: 2024-06-24
permalink: /posts/2024/06/cleveland-wind-tunnel/
tags:
  - baseball
  - Cleveland Guardians
  - home run
---

During the offseason prior to the 2024 season, the Cleveland Guardians decided to put forward a series of renovations accross the stadium. One included their upper deck of seats in right field being revamped to create a new group outing space. This removed an old series of walls and seats, switching to a more open and social look with more access to concession stands. 

<div style="display: flex; justify-content: center;">
  <div style="flex: 1; max-width: 50%; margin-right: 10px;">
    <h3 style="text-align: center;">Old</h3>
    <img src="/images/oldright.png" style="width: 100%; height: auto; display: block;" alt="Illustration of old right field">
    <p style="text-align: center; font-size: 80%;">Illustration courtesy of Cleveland Guardians.</p>
  </div>
  <div style="flex: 1; max-width: 50%; margin-left: 10px;">
    <h3 style="text-align: center;">New</h3>
    <img src="/images/newright.png" style="width: 100%; height: auto; display: block;" alt="Illustration of new right field">
    <p style="text-align: center; font-size: 80%;">Illustration courtesy of David Petkiewicz, cleveland.com.</p>
  </div>
</div>

The Cleveland offense has seen a surge in power numbers across the board and many are beginning to wonder whether this can be attributed to a possible wind tunnel having been created due to the renovations in right field. Many other wonder whether the success can simply be attributed for by an improvement in Cleveland offense from offseason work ethic and improvement. 

Offensive Numbers 
------
This year, Cleveland has clearly been more effective when hitting for power compared to last season which has led them to a top 3 record across the league through their first 75 games. At home, Cleveland is scoring an average of 5.17 runs per game during the 2024 season which as an increase of 1.38 when compared to 2023. On the road, they are scoring 4.95 runs per game in 2024 which is also an increase from last year but only by 0.57 runs. We see a much larger increase of runs per game coming at home. What can this be attributed to?

This year at home, Cleveland is hitting 1.4 home runs per game as opposed to 0.67 home runs in 2023. On the road, they are hitting 0.975 home runs per game in 2024 as opposed to 0.86 in 2023 so we do see another small increase however this doesn't stand out nearly as much as the increase in home runs per game at home. 

<div style="text-align:center;">
  <img src="/images/j_ram_hr.png" style="width:83%;" alt="Image of Jose Ramirez hitting a home run and celebrating.">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Stephanie Scarbrough from the Herald-Star.</p>
</div>

Cleveland's most impressive statistic is their Slugging percentage at home during the 2024 season. They rank 9th best in the MLB at home with a 0.422 SLG. This is an increase in 0.045 from 2023!
They generate this high SLG with mainly home runs as they are last in the MLB at recording 3B and 1B. According to Statcast, the Guardians are in the bottom 2 rankings for both barrel percentage and hard hit percentage across the MLB. 

So, let's take a look at all balls hit in Progressive field throughout this season and the 2023 season for both the Guardians and the opposing teams. This way, we can determine any physical differences in the batted ball distribution before and after the renovations.

Expectd Distance vs. Actual Distance
------
Recently, I read over an article published by Jim Albert and Alan Nathan on this subject to determine whether or not it truly is plausible that a wind tunnel could be creating an offensive explosion in Cleveland. They built a model to determine the probability of a home run for every given batted ball. They then compared the results of this years batted balls to previous years. As I work on my own model and interactive chart, I thought I would share some of their results that I found quite interesting. 

First, we have a basic scatter plot showing the home runs per balls-in-play for Cleveland versus all MLB parks. This being the data from the start of the season through June 15. We can see that in the year of 2024, Cleveland has jumped from the bottom of the league to above the average. This is quite interesting because this doesn't only display the Cleveland offense which means that the balls are flying out at a more extreme rate this year. This is however a small sample size, so it isn't completely decisive. 

<div style="text-align:center;">
  <img src="/images/hr_rate_1.png" style="width:83%;" alt="Image of CLE Home Run Rate">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Jim Albert and Alan Nathan.</p>
</div>

Next, we are shown predicted and actual home run rates for Progressive Field. This is based on a generalized additive model fitted to data from the other MLB parks that was created by Albert and Nathan. I will be attempting to recreate something similar on a wider scale. 

<div style="text-align:center;">
  <img src="/images/hr_rate.png" style="width:83%;" alt="Image of CLE Home Run Rate">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Jim Albert and Alan Nathan.</p>
</div>

We can clearly see that fly balls are traveling further than expected as more home runs are being recorded than predicted. Although, without a large sample size it is not plausible to draw any conclusions this early about any wind tunnels as it could still be related to randomness in the ballpark and different spin variations across the league that hasn't been accounted for in the modeling. 

More Personalized & Interactive Chart Coming Soon
------




Sources
New Image: https://www.cleveland.com/guardians/2024/06/im-at-war-with-progressive-field-wind-tunnel-theory-guards-are-good-period-terry-pluto.html 
Old Image: https://www.perfuzion.com/ballpark-review-progressive-field-cleveland-guardians/ 
Jram: https://www.heraldstaronline.com/sports/local-sports/2024/06/ramirezs-tiebreaking-homer-lifts-guardians/
