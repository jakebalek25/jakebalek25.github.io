---
title: "SMT 2024 Data Challenge"
excerpt: "Uncovering Pre-Pitch Movements by Shortstops Revealing Pitch Tendencies <br/><img src='/images/smt_data_image.png' width='925' height='500'>"
date: "2024-10-10"
collection: portfolio
---

# Uncovering Pre-Pitch Movements by Shortstops Revealing Pitch Tendencies

## Abstract
In baseball, pre-pitch movements by fielders, particularly shortstops, play a crucial role in optimizing positioning and readiness. These movements may also reveal clues about upcoming pitch attributes, potentially providing hitters with a predictive advantage. With little to no previous research published on this topic, there is ground to be gained for MLB teams in conducting research on whether pre-pitch movements do tip pitch attribute tendencies. This study addresses the research gap by analyzing pre-pitch movements by shortstops to determine if they offer insights into the predictability of pitch attributes such as pitch location, pitch type, and vertical break. 

The data provided by the SMT 2024 Data Challenge included ball and player tracking across nearly a season and a half for multiple levels of baseball within a single anonymous organization. To manage complexity, the analysis focused on one level of baseball and focused solely on the shortstop position. Pre-pitch movements were assessed for their predictive power regarding pitch attributes.

The assessment was done using Generalized Linear Models, with separate analysis done for right-handed and left-handed batters. Results indicated that pre-pitch movements do indeed offer modest predictive value for pitch location and pitch type in particular, with models for right-handed hitters performing better than left-handed. The study found that, although better than randomly guessing at an upcoming pitch, the predictions are not highly reliable. Overall, though, the movements by shortstops can offer hitters a slight potential area in predicting a pitches attribute.

The findings highlight the need for further research with the proper data into how different fielders’ pre-pitch movements might signal either pitch attributes or pitch types, emphasizing the importance of analyzing detailed fielding routines and coaching practices.


## 1. Introduction
In baseball, a pre-pitch movement allows fielders to optimize positioning and readiness, significantly impacting their ability to make plays effectively. According to Diamond Dreams Baseball Academy, players develop a strategy for reacting if the ball is put into play. Infielders, especially shortstops, use foot movement and stances to adjust their readiness based on pitch signals.

<div style="text-align:center;">
  <h3 style="text-align: center;">Figure1.1</h3>
  <img src="/images/dusitn_pedroia.jpg" style="width:80%;" alt="Dustin Pedroia pre-pitch movement">
  <p style="text-align:center; font-size:80%;">Dustin Pedroia with his pre-pitch hop into position. If this tennis-hop were to occur by gravitating in a certain direction
depending on the pitch, he would be slightly tipping pitches.</p>
</div>

However, there is limited research on whether these pre-pitch movements tip pitch tendencies to the batter. This leads us to the question, do pre-pitch movement tendencies by shortstops provide clues about the attributes of an upcoming pitch? Through a detailed analysis of pre pitch movements and pitch type outcomes, this research demonstrates that specific movement patterns can be associated with pitch types and locations, thus offering a predictive advantage for hitters.


## 2. Data
For this study, data was obtained from the SMT 2024 Data Challenge, encompassing approximately one and a half seasons of gameplay. The dataset was anonymized to obscure overall demographic details, ensuring that the identities of teams and players remained confidential. The dataset comprises several critical components:
   1. General Game Information: Provides details about each game, including unique identifiers for teams and players.
   2. Ball Position Tracking: Precise tracking of the ball’s position was recorded every 50 milliseconds. It features x, y, and z (height) coordinates, with x and y coordinates relative to the back point of home plate.
   3. Player Position Tracking: Player positions are recorded every 50 milliseconds. This includes x and y coordinates, allowing for detailed analysis of player movements.
   4. Game Play Events: This records key events like pitch throws and ball catches, organized chronologically. It excludes minor events such as hits or outs.
    
### 2.1 Data Processing & Analysis
This study focused on the 4A level to manage the large volume of player positioning data within R Studio’s limits, excluding data from other levels for efficient processing. Additional events were added to the play-by-play data to capture pre-pitch movements, including codes for the ball in the air during the pitch and the phase between plays.

<div style="display: flex; justify-content: center;">
  <div style="flex: 1; max-width: 60%; margin-right: 10px;">
    <h3 style="text-align: center;">Figure 2.1</h3>
    <img src="/images/figure_2_1.png" style="width: 100%; height: auto; display: block;" alt="Illustration of Shortstop 636">
    <p style="text-align: center; font-size: 80%;">This figure displays pre-pitch movement player tracking data for shortstop 636 for a single game when there were only lefty batters at the plate. The colors represent the pitch type thrown after each pre-pitch movement.</p>
  </div>
  <div style="flex: 1; max-width: 60%; margin-left: 10px;">
    <h3 style="text-align: center;">Figure 2.2</h3>
    <img src="/images/figure_2_2.png" style="width: 100%; height: auto; display: block;" alt="Illustration of Shortstop 901">
    <p style="text-align: center; font-size: 80%;">This figure displays pre-pitch movement player tracking data for shortstop 901 for a single game when there were only lefty batters at the plate. The colors represent the pitch type thrown after each pre-pitch movement.</p>
  </div>
</div>

Each shortstop exhibits unique pre-pitch movements: for example, Shortstop 636 moves straight towards home plate with minimal variation, while Shortstop 901 moves back towards the middle of the field. The study analyzes how these movements might predict pitch attributes.

To manage the data, only timestamps related to shortstops were retained. Missing values in IDs and player position tracking data were addressed to ensure the dataset's integrity. The cleaned dataset included 764,760 observations over 10,504 pitches at the 4A level.


## 3. Methodology
This study uses a quantitative research design to analyze the correlation between pre-pitch player position tracking and upcoming pitch attributes.
First, a new variable identified whether each pitch was thrown on the left or right side of the strike zone, measuring the horizontal ball position (x) at the closest point to the plate (y=0). Due to data being recorded every fifty milliseconds, some data points were missing, including instances where the ball crossed the plate. To combat this, the x location was determined at the closest point to the plate in which the ball was recorded. This was the first major attribute towards predicting a pitch.

A new variable was created to calculate pitch speed. Using J.J. Cooper's method from Baseball America, velocity was measured at 50 feet from the plate, as traditionally done in MLB until recently. Due to missing data when the ball is exactly 50 feet from the plate, speed was instead measured at data points between 55 and 45 feet, covering 99% of the pitches. Speed was calculated using the formula Distance/Time in feet per second and then converted to miles per hour (MPH) by multiplying by approximately 0.68.

Based on the speed of each pitch thrown, a binary variable was calculated to classify each pitch as either an off-speed pitch or a fastball variant. A pitch was classified as a fastball if it fell within the top 7% of each pitcher’s velocity range, ensuring that all fastball pitches had a mean speed of 91.6 mph. This is just below the MLB average of around 92 mph, providing a solid benchmark. This binary classification of pitch type is a key attribute in the analysis.

Vertical break for each pitch was calculated by determining when the pitch was in the air and gathering the ball_position_z measurements to measure the change in height. The change in heights was identified as the vertical break. Once this was calculated, the 50th percentile of the vertical break was determined. A new variable was created using percentile-based binarization to classify pitches as having a high vertical break versus a low vertical break at the 50th percentile, which is another key attribute in the analysis.

A new variable was created to label the location where each ball was hit, categorizing it as either the left side, up the middle, or the right side. Based on hit charts from FanGraphs, 15- degree angles were used to split the zones between left center field and right center field, effectively representing the three batting zones. The data was then filtered based on x and y coordinates to determine the zone for each hit.

A K-Means Clustering approach was used to predict batter handedness, categorizing batters as right-handed or left-handed while excluding switch hitters. The model used pitch location, pitch speed, and ball acquisition coordinates to predict handedness, hypothesizing that pitch location influences whether a batter hits to the left or right field. 

Generalized Linear Models (GLMs) were then developed to predict pitch attributes based on pre-pitch movements. The data was analyzed separately for right-handed and left-handed hitters, as each group was expected to yield different results. The models predicted pitch location, pitch type (fastball or off-speed), and vertical break (high or low) using pre-pitch movements. Performance was evaluated using Accuracy, Recall, Precision, and F1 Score to assess how well pre-pitch movements can predict pitch attributes and the effectiveness of each model.












