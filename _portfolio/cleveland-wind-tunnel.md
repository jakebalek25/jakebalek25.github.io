---
title: "Progressive Field 'Wind-Tunnel'"
excerpt: "Modeling Hit Distance Predictions to Detect 'Wind-Tunnel' <br/><img src='/images/progressive_field.png' width='925' height='500'>"
date: "2024-07-09"
collection: portfolio
---

# Recent Cleveland Rennovations
---
During the 2023-2024 offseason, the Cleveland Guardians decided to make multiple renovations to Progressive Field. The renovations took place in 5 different areas throughout the stadium. The locations included beyond right field, down the left field line and directly behind home plate. In right field, they added the 'Right Field Paul Davis Pennant District' which features a new open-air, group outing area with concession stands. Previously, there had been another deck of seats and a wall blocking off any airflow to the concession stands. 

To begin the first half of the 2024 season, the new panoramic angles in right field have offered a view to one of the most high powered offenses in the league. Through Cleveland's first 81 games, they have the 4th highest scoring offense in the league by averaging 5 runs per game. This has helped propel the team to the best record in the league at 52-29. On the flip side, Cleveland's pitching is allowing the 6th most home runs per 9 innings at home this season. High offensive numbers for all teams playing in Cleveland has highlighted an underlying question that has been trending lately: “Have Progressive Field upgrades created a home run ‘wind tunnel’?”.


# Determining Whether or Not a 'Wind-Tunnel' Exists
---
An increase in offensive production and home run numbers at Progressive Field during the 2024 season has sparked speculation about the presence of a ‘wind-tunnel’ effect. To determine whether this phenomenon is occurring or if the changes are simply due to the Guardians' performance, I decided to research further.

After reading multiple articles on predicting the distance of a batted baseball by Alan Nathan, Jim Albert, Joe Noga, and another by Cameron Grove, I attempted to replicate some of their ideas and draw my own conclusions.

Before we dive in, it must be noted that the “actual home run rate” used in each model was slightly higher than it should have been due to a small number of missing values for launch speed and launch angles within our data. This discrepancy caused a slight difference from the actual home run rate in real time.

# Comparing Actual Home Run Rates
---
Similar to the research conducted by Alan Nathan and Jim Albert, this analysis begins by comparing home run rates across multiple years at Progressive Field. To start, let's examine how the home run rate at Progressive Field has compared to the rest of MLB over the past few years.

IMAGE 1 
<div style="text-align:center;">
  <img src="/images/IMAGE1" alt="Home Run Rate Comparison: Cleveland vs. MLB">
  <p style="text-align:center; font-size: smaller;">The chart shows the Home Run Rate for all balls in play (BIP) from 2020-2024 with each BIP correlating to the responding year. The Cleveland rate includes all BIP at Progressive Field, while the MLB rate covers all other parks. Both the Guardians' and opposing teams' BIP are included to.</p>
</div>

Spanning from the 2020 season to the current 2024 season, Cleveland has had two seasons in which the home run rate at Progressive Field was above the league average. In 2021, the home run rate at Progressive Field was nearly 0.5% higher than the league average. After 2021, the rate dropped significantly below the league average until the current 2024 season. Now, Progressive Field is again seeing home run rates soar above the league average, but at an even larger margin. This season, the home run rate at Progressive Field is nearly 1% higher than the league average—double the margin from 2021. These large, linear changes in home run rates at Progressive Field raise the question: Are the home run rates due to the Guardians' performance each year, or is there truly a 'wind-tunnel' effect in Cleveland post-renovations?


# Predicting Home Run Rates



# Comparing Actual Hit Distance to Predicted Hit Distance



# Conclusions



Sources
------
Cover image : https://guardians.fanportal-mlb.com/renovations/
