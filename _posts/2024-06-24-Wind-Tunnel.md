---
title: "Has Cleveland Created A 'Wind-Powered' Long Ball Haven With Their Recent Stadium Renovations?"
date: 2024-06-24
permalink: /posts/2024/06/cleveland-wind-tunnel/
tags:
  - baseball
  - Cleveland Guardians
  - home run
---

During the offseason preceding the 2024 season, the Cleveland Guardians decided to undertake a series of renovations across the stadium. One major change involved the upper deck of seats in right field, which was revamped to create a new group outing space. This renovation involved removing old walls and seats, transitioning to a more open and social layout with increased access to concession stands

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

The Cleveland offense has shown a surge in power numbers across the board, prompting speculation about whether this can be attributed to a potential wind tunnel created by renovations in right field. Others speculate that the team's success simply reflects improvements in their offseason work ethic and overall offensive capabilities. 

Offensive Numbers 
------
This year, Cleveland has noticeably improved their power hitting compared to last season, leading them to hold a top 3 record across the league after their first 75 games. At home, Cleveland is averaging 5.17 runs per game in the 2024 season, an increase of 1.38 runs compared to 2023. On the road, they are scoring 4.95 runs per game in 2024, up by 0.57 runs from last year. The larger increase in runs per game at home raises the question: what is contributing to this difference?

At home this year, Cleveland is hitting an average of 1.4 home runs per game, compared to 0.67 home runs in 2023. On the road, they are hitting 0.975 home runs per game in 2024, slightly up from 0.86 in 2023. However, the increase in home runs per game at home is significantly more pronounced than on the road.

<div style="text-align:center;">
  <img src="/images/j_ram_hr.png" style="width:83%;" alt="Image of Jose Ramirez hitting a home run and celebrating.">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Stephanie Scarbrough from the Herald-Star.</p>
</div>

Cleveland's most impressive statistic in the 2024 season is their slugging percentage (SLG) at home, where they rank 9th best in MLB with a .422 SLG. This marks a significant increase of .045 from 2023. The Guardians achieve this high SLG primarily through home runs, as they rank last in MLB in both triples (3B) and singles (1B). According to Statcast, the Guardians also rank in the bottom two for barrel percentage and hard-hit percentage across the league.

To further analyze this, let's compare all balls hit at Progressive Field between the 2023 and 2024 seasons for both the Guardians and visiting teams. This comparison will help us identify any physical differences in batted ball distribution before and after the renovations.

Expectd Distance vs. Actual Distance
------
Recently, I reviewed an article by Jim Albert and Alan Nathan exploring whether a wind tunnel effect could be contributing to an offensive surge in Cleveland. They constructed a model to assess the probability of a home run for each batted ball and compared this year's data with previous seasons. As I develop my own model and interactive chart, I found some of their results particularly intriguing.

One notable finding is depicted in a basic scatter plot illustrating home runs per balls-in-play for Cleveland compared to all MLB parks, based on data up to June 15 of the 2024 season. Cleveland has markedly risen from being below league average to above average this year. This trend suggests a notable increase in home runs, not just attributable to Cleveland's offense but possibly indicating a higher rate of balls leaving the park. However, it's important to note that this conclusion is drawn from a relatively small sample size, which limits its decisiveness.

<div style="text-align:center;">
  <img src="/images/hr_rate_1.png" style="width:83%;" alt="Image of CLE Home Run Rate">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Jim Albert and Alan Nathan.</p>
</div>

Next, I examined the predicted and actual home run rates specifically for Progressive Field, using a generalized additive model developed by Albert and Nathan with data from other MLB parks. I aim to replicate a similar analysis on a broader scale.

<div style="text-align:center;">
  <img src="/images/hr_rate.png" style="width:83%;" alt="Image of CLE Home Run Rate">
  <p style="text-align:center; font-size:85%;">Illustration courtesy of Jim Albert and Alan Nathan.</p>
</div>

It's evident that fly balls are traveling farther than anticipated, resulting in more home runs than predicted. However, drawing conclusions about the presence of wind tunnels at this stage is not plausible due to the limited sample size. Factors such as randomness in ballpark conditions and varying spin rates across the league, which may not have been fully accounted for in the modeling, could also contribute to these observations.




!! More Personalized & Interactive Chart Coming Soon !!
------
After reading multiple articles related to predicting the distance of a batted baseball by Alan Nathan, Jim Albert and another by Cameron Grove, I decided to try and replicate some of their ideas. I used similar play by play data from the 2024 season that I scraped using baseballr. With the data I filtered out only instances in which the ball was hit to the right side of the field, was considered to be a fly ball and traveled more than 120 feet. This ensured that the data relating to Progressive Field and all other ballparks could display the effects of strictly right field's 'Wind-Tunnel'. First, I trained a GAM predictive model on all of the play by play data on fly balls to right field throughout the 29 other ballparks in the MLB during the 2024 season after filtering out all data from within Progressive Field. The model's independent variables consisted of Launch Angle and Launch Speed. These variables were most commonly used among other researchers studies so I wanted to recreate a similar model. 
Next, I used the model's findings to predict hit distances within Progressive Field on fly balls to right field. After finding my predictions, I compared them to the actual results. Theoretically, a 'Wind-Tunnel' would mean that the actual distances were further than the predicted distances because the predictions were based on other stadiums having no wind tunnels to right. 

Graph showing Predicted Distances

Within our findings, we saw that Progressive Field did indeed see



Sources
------
The Herald Star. (2024, June 25). Ramírez’s tiebreaking homer lifts guardians. heraldstaronline.com. https://www.heraldstaronline.com/sports/local- 
    sports/2024/06/ramirezs-tiebreaking-homer-lifts-guardians/ 
    
Perdue, S. (2023, June 18). Ballpark Review: Progressive field (cleveland guardians). Perfuzion. https://www.perfuzion.com/ballpark-review-progressive-field- 
    cleveland-guardians/ 
    
Pluto, T. (2024, June 15). I’m at war with the Progressive Field “wind tunnel” theory. the Guardians are good, period! – Terry Pluto. cleveland.com. 
    https://www.cleveland.com/guardians/2024/06/im-at-war-with-progressive-field-wind-tunnel-theory-guards-are-good-period-terry-pluto.html 
    
Albert & Nathan article
--
Searle, G. (2024, June 25). Balls are traveling farther in 2024 in Progressive Field. Baseball Prospectus. 
    https://www.baseballprospectus.com/news/article/91708/balls-are-traveling-farther-in-2024-in-progressive-field/ 
