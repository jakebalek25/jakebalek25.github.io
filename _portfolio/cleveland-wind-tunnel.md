---
title: "Progressive Field 'Wind-Tunnel'"
excerpt: "Modeling Distance Predictions to Detect 'Wind-Tunnel' <br/><img src='/images/progressive_field.png'>"
date: "2024-07-01"
collection: portfolio
---

# Recent Cleveland Rennovations
---
During the offseason between the 2023 and 2024 seasons, the Cleveland Guardians decided to make multiple renovations to Progressive Field. These included 5 different areas throughout the stadium. The locations included beyond right field, down the left field line and directly behind home plate. In right field they added the 'Right Field Paul Davis Pennant District' which features a new open-air, group outing area. Previously, there had been another deck of seats and a wall blocking off any airflow below said seats. 


This year



After reading multiple articles related to predicting the distance of a batted baseball by Alan Nathan, Jim Albert and another by Cameron Grove, I decided to try and replicate some of their ideas. I used similar play by play data from the 2024 season that I scraped using baseballr. With the data I filtered out only instances in which the ball was hit to the right side of the field, was considered to be a fly ball and traveled more than 120 feet. This ensured that the data relating to Progressive Field and all other ballparks could display the effects of strictly right field's 'Wind-Tunnel'. First, I trained a GAM predictive model on all of the play by play data on fly balls to right field throughout the 29 other ballparks in the MLB during the 2024 season after filtering out all data from within Progressive Field. The model's independent variables consisted of Launch Angle and Launch Speed. These variables were most commonly used among other researchers studies so I wanted to recreate a similar model. 
Next, I used the model's findings to predict hit distances within Progressive Field on fly balls to right field. After finding my predictions, I compared them to the actual results. Theoretically, a 'Wind-Tunnel' would mean that the actual distances were further than the predicted distances because the predictions were based on other stadiums having no wind tunnels to right. 

Graph showing Predicted Distances

Within our findings, we saw that Progressive Field did indeed see



Sources
------
Cover image : https://guardians.fanportal-mlb.com/renovations/
