---
title: "Progressive Field 'Wind-Tunnel'"
excerpt: "Modeling Distance Predictions to Detect 'Wind-Tunnel' <br/><img src='/images/progressive_field.png'>"
date: "2024-07-01"
collection: portfolio
---

# Recent Cleveland Rennovations
---
During the 2023-2024 offseason, the Cleveland Guardians decided to make multiple renovations to Progressive Field. The renovations took place in 5 different areas throughout the stadium. The locations included beyond right field, down the left field line and directly behind home plate. In right field, they added the 'Right Field Paul Davis Pennant District' which features a new open-air, group outing area with concession stands. Previously, there had been another deck of seats and a wall blocking off any airflow to the concession stands. 

To begin the first half of the 2024 season, the new panoramic angles in right field have offered a view to one of the most high powered offenses in the league. Through Cleveland's first 81 games, they have the 4th highest scoring offense in the league by averaging 5 runs per game. This has helped propel the team to the best record in the league at 52-29. On the flip side, Cleveland's pitching is allowing the 6th most home runs per 9 innings at home this season. High offensive numbers for all teams playing in Cleveland has highlighted an underlying question that has been trending lately: “Have Progressive Field upgrades created a home run ‘wind tunnel’?”.


# Determining Whether or Not a 'Wind-Tunnel' Exists
---
Speculation about a 'wind-tunnel' in Cleveland has led to people connecting the increase of offensive production and home runs for the 2024 season.  

To determine whether or not a 'wind-tunnel' has helped the flight of the baseball in Cleveland, we must compare the actual distance of each traveled baseball to the predicted distance of the same hit baseball.

After reading multiple articles related to predicting the distance of a batted baseball by Alan Nathan, Jim Albert, Joe Noga and another by Cameron Grove, I decided to try and replicate some of their ideas. I decided that 

I used similar play by play data from the 2024 season that I scraped using baseballr. With the data I filtered out only instances in which the ball was hit to the right side of the field, was considered to be a fly ball and traveled more than 120 feet. This ensured that the data relating to Progressive Field and all other ballparks could display the effects of strictly right field's 'Wind-Tunnel'. First, I trained a GAM predictive model on all of the play by play data on fly balls to right field throughout the 29 other ballparks in the MLB during the 2024 season after filtering out all data from within Progressive Field. The model's independent variables consisted of Launch Angle and Launch Speed. These variables were most commonly used among other researchers studies so I wanted to recreate a similar model. 
Next, I used the model's findings to predict hit distances within Progressive Field on fly balls to right field. After finding my predictions, I compared them to the actual results. Theoretically, a 'Wind-Tunnel' would mean that the actual distances were further than the predicted distances because the predictions were based on other stadiums having no wind tunnels to right. 

Graph showing Predicted Distances

Within our findings, we saw that Progressive Field did indeed see



Sources
------
Cover image : https://guardians.fanportal-mlb.com/renovations/
