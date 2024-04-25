---
title: "2024 SABR Diamond Dollars Case Competition"
excerpt: "Determining the Value of a Foul Ball <br/><img src='/images/foulBall.jpg'>"
date: "2024-04-23"
collection: portfolio
---

[![SABR project slide show](/images/DiamondDollarsCaseCompSlide.png)](/files/DiamondDollarsCaseCompSlides.pdf)
The link to the slideshow can be found by clicking on the image. 

The prompt was to establish a set of criteria enabling competitors to create a metric defining the value of a given foul ball. The next step was to determine whether it benefitted the pitcher or hitter, and by how much.

We then decided we wanted to create a different metric for both hitters and pitchers to determine when a foul ball was beneficial towards the offense or defense. We calculated out probabilities based on the count and then created a supplement metric for the foul ball metric with xBA and the out probabilities modeled. We then created a Naive Bayes model to connect all of the supplements into one metric.

Our metric aimed to reward batters for fouling off pitches with a higher probability of being called a strike and punish batters for fouling off pitches with a lower probability of being called a strike. 

I created a basic shiny app to display our results in a more interactive way. Click on the image for more!
[<img src="/images/BasicShinyApp.png" alt="Homescreen of Shiny App">](https://jjbalek.shinyapps.io/Case_Comp_Shiny_App/)
Reminder: There was only one week to complete the case competition and the shiny app was the least of priority on the last days so it is quite basic!
