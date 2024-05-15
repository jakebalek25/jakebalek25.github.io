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

This week, while watching the Chicago Cubs take on the Pittsburgh Pirates, a particular situation caught my attention: a runner positioned on 2nd base with zero outs. Despite the Cubs struggles throughout the regular 9 innings, their performance notably improved during their long opportunity in extra innings as they demonstrated a newfound ability to score with ease in this situation. This observation prompted me to think about several inquiries regarding teams and hitters strategy in these pivotal moments. 
- In extra innings, teams are more focused on scoring the runner on second rather than extending an inning. Does this change how teams approach the situation such as electing to sacrifice the runner over more often? 
- When not sacrificing, do hitters try to hit the ball to the outfield or on the ground more often?
- How often are hitters successful in this situation?

<div style="text-align:center;">
  <img src="/images/Cubs-Pirates-Baseball-33-1687355326.png" alt="Illustration of Cubs vs. Pirates">
</div>

Utilizing play-by-play data from Baseball Savant covering the years 2020-2023, I conducted an analysis to gain insights into hitters and teams performance/strategy in this situation. The study focuses specifically on situations where a runner occupies 2nd base and there are zero outs in the inning, resembling the beginning of an extra inning. By examining this scenario, the goal is to discern how teams and hitters adapt their strategies when faced with the unique dynamics of extra innings compared to regular gameplay. 


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

The delta home win expectancy tells us the change in percent chance that the home team will win based on the score, inning, outs, runners on base and other situational factors that could affect the score. In this situation, we only have the change in the home win expectancy. So, when the delta home win expectancy is positive in the bottom half of an inning, we can conclude that it is a good at-bat. The opposite goes for the away team. When the delta home win expectancy is negative in the top half of an inning, we can conclude that the result is a good at-bat for the away team. 

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
<div style="width: 95%; margin: 0 auto; display: flex; justify-content: space-between;">
  <figure>
    <img src="/images/hittypesreg.png" alt="Pie chart showing the distribution of hit types when an out is recorded on a ball in play during regular innings" style="width: 100%;">
    <figcaption>Regular Innings</figcaption>
  </figure>

  <figure>
    <img src="/images/hittypesextras.png" alt="Pie chart showing the distribution of hit types when an out is recorded on a ball in play during extras innings" style="width: 100%;">
    <figcaption>Extra Innings</figcaption>
  </figure>
</div>

The pie charts show each batted ball during both regular innings and extra innings with a runner on solely 2nd and no outs. This displays trends among how hitters tend to try and hit the ball depending on what inning the game may be in. We can see that in extra innings, hitters tend to try and keep the ball on the ground more than in regular innings. This is likely to try and advance the go ahead runner to either third or home rather than hitting the ball in the air and lessening the chance the runner can advance. 

On another note, according to delta home win expectancy, there are many more "good" at-bats during extra innings with a runner on 2nd and no one out. During regular innings, only 33.6% of at-bats result in a "good" at-bat. In extra innings, 47.4% of at-bats result in "good" at-bats. This could be because within the last inning of a game a single run is much more crucial than in the first few innings of a game. So, by sacrificing a runner to third, it would be worth more delta home win expectancy. 

Conclusion
------
Overall, teams should look into trying to sacrifice the runner to third more often than allowing a hitter to swing away in late-game situations. A runner at third with one out is more valuable than a runner at second with no outs in a late game situation. In extra innings, a run is much more important than an out as opposed to earlier in the game. 

Other ideas: 
  - Take a look at how hitters may respond depending on the score.
  - Take a look at how each indivudual team goes about the situation with a runner on 2nd and no outs.
  - Take a look at which batter counts generate higher delta win expectancy changes.
  - Take a look at other situations rather than just runner on second with no outs.
  - What other situations require lots of strategy outside of hitting the ball?
