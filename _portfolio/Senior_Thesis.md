---
title: "Evaluating the Relationship Between Pitch Location and Batted Ball Directional Success at the MLB Level"
excerpt: "Are MLB Hitters Pulling the Ball too Often? <br/><img src='/images/wOBA_Differences_in_Pull_Oppo.png' width='650' height='300'>"
date: "2025-07-14"
collection: portfolio
---

![Visual displaying batted ball expected wOBA on piches inside vs. outside and where they should be hit](/images/wOBA_Differences_in_Pull_Oppo.png)

## Abstract
For years, hitters have been taught to “hit the ball where it’s pitched,” but recent trends in the MLB have revealed the advantages of pulling the ball. This study dives into the relationship between pitch location, pitch type and batted ball direction to better understand how hitters achieve the most successful outcomes. Using modeling, machine learning, and visualizations, the results show that pulling the ball on pitches throughout the strike zone, even outside corner, tends to lead to better offensive production. These findings challenge the traditional narrative and suggest that teams should teach hitters to hit the ball out in front of their body to pull the ball for more power. 


## 1. Introduction
Growing up playing baseball as a right-handed hitter, I was always taught to “hit the ball where it’s pitched”, meaning that I pull inside pitches to left and hit outside pitches to right field. I always felt that when I tried to hit the ball the other way, I was losing power and felt more confident pulling the ball. 

In a Fangraphs article by Ben Perry in 2022, he questioned the phrase “hit it where it’s pitched” which inspired this study to be conducted on a deeper level. In another recent study conducted by Mike Petriello, he concluded that hitting the ball 36 inches out in front of the body’s center of mass leads to the most success in terms of power.  

This shift in hitting has led teams to rethink conventional ideas about swing approach. There is now greater emphasis on promoting aggressive swings designed to pull the ball except in specific situations or pitch locations that demand a more defensive approach. Hitters are being trained to hunt pitches they can drive out front. These adjustments reflect a deeper understanding of how contact point, swing path, and bat speed all interact to influence batted ball outcomes.

By examining correlations through visualization, generalized additive models and XGBoost machine learning techniques, this research analyzes how different pitch characteristics affect the success of pulled, straightaway, and opposite-field contact. By identifying patterns in batted ball behavior based on pitch location and type, the study seeks to provide insights that could help hitters, refine approaches to maximize offensive performance. 

## 2. Literature Review
In the past, there has been research dedicated to understanding at what point hitters should make contact with the ball in terms of success, but there hasn’t been much research on where a ball should be hit based on where it was pitched in the zone. To understand what this article examines, let’s take a step back to understand what has already been researched. 

### 2.1 Similar Baseball Modeling Techniques
To better understand how hitters hit the ball a certain way, we must first understand how researchers understand the game and have gone about this topic in the past. Analytics in baseball force teams to ask better questions and push old narratives that have been around in baseball for decades. For example, what if we could predict a batted ball’s outcome based on swing mechanics and batted ball metrics. 

Albert (2018) did just that by using Generalized Linear Models (GLM) to forecast hit probability based on launch angle, exit velocity and spray angle. His findings revealed that spray angle was a key contributor when predicting ground ball outcomes and a significant predictor of whether or not it resulted in a hit. The direction of balls hit in the air proved to be less critical. Albert’s study used GLM’s and visualization to display how important spray angle is when determining how successful a hitter will be with a certain batted ball. 

In other light, defense hasn’t been left behind during the transition of data into the baseball world. Jensen, Shirley, and Wyner (2009) shifted the analytical spotlight to analyzing fielders by using Bayesian Hierarchical models on batted ball data. By borrowing strength across positions and players, they crafted a fair set of rankings and assessment of fielding performance. This study provides a method for evaluating complex aspects of player performance. 

Both aproaches form a foundation for understanding baseball in a new light. It’s not about whether something happened, but rather why or how often it should have happened. This thinking opens a door for a deeper dive into how hitters can maximize outcomes by targeting pitch types, locations and directions. 






