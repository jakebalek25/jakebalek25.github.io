---
title: 'Hitting With Runner on 2nd & No Outs'
date: 2024-05-13
permalink: /posts/2024/05/hitting-runner-on-second/
tags:
  - baseball
  - hitting strategy
  - extra innings
  - Chicago Cubs
---

This week, while watching the Chicago Cubs play the Pittsburgh Pirates, I couldn't help but think about how hitters approach situations when there is a runner on second base with no outs. The Cubs had little success during the regular 9 innings. However, in extras they were able to score quite easily. I had a couple ideas and questions about the situation. 
- In extra innings, teams are more focused on scoring the runner on second rather than extending an inning. Does this change how teams approach the situation such as electing to sacrifice the runner over more often? 
- When not sacrificing, do hitters try to hit the ball to the outfield or on the ground more often?
- How often are hitters successful in this situation?

<div style="text-align:center;">
  <img src="/images/Cubs-Pirates-Baseball-33-1687355326.png" alt="Illustration of Cubs vs. Pirates">
</div>

Using play-by-play Baseball Savant data spanning from 2020-2023, I was able to prepare some visuals to better understand how hitters have performed in this situation. This study only examines situations in which there is a runner solely on 2nd base with 0 outs to mimmick the start of an extra inning. The goal is to determine how teams and hitters decide to play the situation differently in extra innings versus a regular inning. 


Regular Innings
------
The goal of any team during the regular 9 innings during a typical baseball game is to extend an inning as long as they can in order to score more runs. It may almost seem as though sacrificing a runner to third by bunt is a waste of an out so many teams decide not to put this play into action. Therefore, hitters are called upon to produce a successful at-bat and either score the runner or hit the runner to third base while trying to reach base. 

<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/secondbasecount1.png" alt="Table showing the distribution of events for the at-bat following in regular innings" style="width: 100%;">
  <figcaption style="margin-top: 10px;">The "other" column incorporates a catcher interference, fielding error, hit by pitch, or a triple play. These events were either very rare or out of the hitter's control.</figcaption>
</figure>

<figure style="width: 90%; margin: 0 auto; text-align: center;">
  <img src="/images/secondbasecount.png" alt="Table showing the distribution of events for the at-bat following in regular innings" style="width: 100%;">
</figure>

We see that teams tend to allow their hitters swing away in this situation as sacrifice bunts only account for roughly 4% of our total population. However, 30% of the time, hitters extend the inning just as they are asked to do by either recording a single, double, triple, home run or walk. In other words, a hitter will score the runner from 2nd around 20% of the time which is a pretty good rate. So is hitting a sacrifice fly or even sacrifice bunting it in this situation worth it?

Lets dive deeper by looking at how each event affects the delta home win expectancy!

The delta home win expectancy tells us the change in percent chance that the home team will win based on the score, inning, outs, runners on base and other situational factors that could affect the score. In this situation, we only hace the change in the home win expectancy. So, when the delta home win expectancy is positive in the bottom half of an inning, we can conclude that it is a good at-bat. The opposite goes for the away team. When the delta home win expectancy is negative in the top half of an inning, we can conclude that the result is a good at-bat for the away team. 

<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/deltahomewinreg.png" alt="Table showing the distribution of events for within a good or bad at bat" style="width: 100%;">
</figure>

The table shows that by adding win expectancy as a result of a single at-bat, it is considered a good at-bat. Generally, getting on base is the best for delta home win expectancy. However, it must be noted that sac bunt and sac fly are also considered a good at-bat during regular innings in this situation despite recording an out. 


Extra Innings
------
The rule of a runner starting on second base was implimented in the 2020 shortened season and fully adopted later. The importance of scoring the runner at 2nd is crucial because it is hard to stop once on defense. A strikeout is the worst possible scenario that can occur in the leadoff spot during an extra inning because the ball isn't put into play meaning the runner has a 0% chance of either scoring or advancing a base. Runs are much more valuable in extra innings because it is a tie game so taking the lead by one can be all a team needs to win the game. By starting the inning with a "good" at-bat, teams are much more likely to raise the delta win expectancy. 

<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/secondbasecountextras1.png" alt="Table showing the distribution of events for the at-bat following in extra innings" style="width: 100%;">
  <figcaption style="margin-top: 10px;">The "other" column incorporates a catcher interference, fielding error, hit by pitch, a triple play or a stolen 3rd base. These events were either very rare or out of the hitter's control.</figcaption>
</figure>

<figure style="width: 90%; margin: 0 auto; text-align: center;">
  <img src="/images/secondbasecountextras.png" alt="Table showing the distribution of events for the at-bat following in extra innings" style="width: 100%;">
</figure>

In extra innings, a hitter safely reaches base by single, double, triple, home run, or walk over 28% of the time. By recording a base hit, the runner will likely score which accounts for 21% of the data. However, what is interacting is that hitters tend to sac bunt 9.5% of the time. Teams elect to attempt to sacrifice the runner to third in attempt to score the go ahead run in extra innings. This is 5% higher than in regular innings which means that teams value a runner at third with one out more than a runner at 2nd with 0 outs. Another interesting note is that the strikeout rate dropped 1.5% as teams are telling their hitters the ball must be in play because a strikeout in this situation could lose the game rather than trying to hit a ball to the right side with 2 strikes. 

<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/deltahomewinextras.png" alt="Table showing the distribution of events for within a good or bad at bat" style="width: 100%;">
</figure>

This is quite possibly the most interesting piece of information in the study! The number of "good" at-bats during extra innings in this situation is much higher at 47.5% when in the specific situation. This could be because every at-bat has a lot more weight in terms of delta win expectancy. Scoring a run to take the lead late in the game means more than scoring a run to take the lead in an early inning however, the chart wasn't weighted to measure that. It was simply made to measure the counts of when a "good" or "bad" at-bat was recorded. 


Comparing Both Situations
------
<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/hittypesreg.png" alt="Pie chart showing the distribution of hit types when an out is recorded on a ball in play during regular innings" style="width: 100%;">
</figure>

<figure style="width: 75%; margin: 0 auto; text-align: center;">
  <img src="/images/hittypesextras.png" alt="Pie chart showing the distribution of hit types when an out is recorded on a ball in play during extras innings" style="width: 100%;">
</figure>

We can look at both pie charts to determine when hitters may be trying to hit the ball differently.

We can also look into how teams are much more likely to attempt a sacrifice bunt by comparing the distribution of events during extra innings and regular innings.

Whats interesting is that, according to delta home win expectancy, there are many more "good" at-bats during extra innings with a runner on 2nd and no one out. During regular innings, only 33.6% of at-bats result in a "good" at-bat. In extra innings, 47.4% of at-bats result in "good" at-bats. This could be because within the last inning of a game a single run is much more crucial than in the first few innings of a game. So, by sacrificing a runner to third, it would be worth more delta home win expectancy. Overall, teams should look into trying to sacrifice the runner to third more often than allowing a hitter to swing away in late-game situations. A runner at third with one out is more valuable than a runner at second with no outs in a late game situation. 

