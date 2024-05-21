---
title: 'Swinging Too Hard?'
date: 2024-05-19
permalink: /posts/2024/05/swinging-too-hard/
tags:
  - baseball
  - statistic leader
  - strikeout
---

This year, the MLB has implimented new bat-tracking technology using a Hawk-Eye system which utlizes 12 cameras positioned around each MLB stadium that capture publicly available data. It offers very unique insight into why some hitters may be better than others including bat speed to the sweet spot at contact. 

Something that I found to be intriguing recently was that the leaderboard for bat speed reminded me a lot of players who had high strikeout numbers to begin the 2024 season. With this in mind I bagan to breakdown the list and realize that other than a few outliers, most of the players have had high strikeout numbers in years past. 

<div style="text-align:center;">
  <img src="/images/savant_leaderboard.png" style="width:83%;" alt="Illustration of 2024 Swing Speed Leaderboard">
  <p style="text-align:center;">Illustration of 2024 Swing Speed Leaderboard from Baseball Savant.</p>
</div>

All of the names near the top of the list are players you would expect to have some of the highest exit velocities because of how hard they swing the bat. However, there are some other trends that are starting to stick out among these hitters. 

Determining Statistical Trends Based on Swing Speed
------
Among the qualified 166 hitters during the beginning of the 2024 season, multiple trends were found relating to swing speed affecting swing and miss numbers. I decided to make some simple scatterplot graphs to visualize the distribution of data across the league to see whether or not this was an actual issue. 

<div style="text-align:center;">
  <img src="/images/swingspeed_kpct.png" alt="Illustration of 2024 Swing Speed vs. Strikeout Percentage">
  <p style="text-align:center;">Illustration created using R Studio ggplot2 package.</p>
</div>

The first chart shows the relationship between the new data of average swing speed and each batters corresponding strikeout percent. The trend line shows a positive slope as we move from left to right. This means that across the league, as a batter's average swing speed increases, so does their strikeout percentage. 

We can see some outliers such as Giancarlo Stanton on the far right who is also known for his extreme power while we see Luis Arraez on the opposite side. He is typically known for his contact hitting and lower exit velocities.

<div style="text-align:center;">
  <img src="/images/swingspeed_whiffpct.png" alt="Illustration of 2024 Swing Speed vs. Whiff Percentage">
  <p style="text-align:center;">Illustration created using R Studio ggplot2 package.</p>
</div>

Next, we see the relationship between average swing speed and whiff percentage. Once again, the higher the average swing speed is, the higher the whiff percentage that transpires. This could mean that hitters in these situations may swing out of their shoes too much trying to crush the ball rather than keeping their swing short and staying through the ball.

<div style="text-align:center;">
  <img src="/images/hardswing_kpct.png" alt="Illustration of 2024 Hard Swing vs. Strikeout Percentage">
  <p style="text-align:center;">Illustration created using R Studio ggplot2 package.</p>
</div>

Finally, although the incline is smaller, there is still a positive trend: batters who record hard swings, as measured by Hawk-Eye, tend to strike out more often. This could be player's bats are moving through the zone quicker. When in the zone for less time it is harder to not only hit the ball but also control the bat. 


Conclusion
------
Overall, hitters who swing harder show a higher likelieness to strikeout more often. They are likely power hitter archetypes so this would make sense as this player usually has a good amount of strikeouts to go with their home runs and hard hit balls. 

This makes me wonder, will Hawk-Eye and bat speed statistics be the new change in the MLB over the next few years just as Statcast was with exit velocity?
