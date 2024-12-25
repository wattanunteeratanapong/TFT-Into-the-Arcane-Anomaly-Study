# TFT-Set-13-Anomaly-Study
Have you ever wonder how many time do we have to roll until we found the anomaly that we're looking for in TFT Set13? <br><br>
![TeamfightTactics_Set13_IntotheArcane_KeyVisual_Powder_Sevika_Vander_Vi](https://github.com/user-attachments/assets/cf9b3a1e-c547-4252-b89f-c8ebfa2e9658)


## Overview
In this experiment we gonna test both patch 14.23 and 14.24 <br>
The different between these patch anomaly system is <br>
Patch 14.23 : The anomaly that have already been roll are not gonna appear again in the pool <br>
Patch 14.24 : The anomaly that have already been roll might be able to appear again in the pool <br>
If we compare this to the Probability Patch 14.23 would be Dependent Trail, and Patch 14.24 would be Independent Trial <br>
Time of simulation is around 10 million time for getting close to the theoratical probability as much as possible<br>
<br>


## Hypothesis
### Patch 14.23
"Hypergeometric Random Variable" (Dependent Trial) <br>
P(K N) is a probability of success k time in n trial (order doesn't matter) <br>
P(K N) = KCk × (N-K)C(n-k) / NCn <br>
P(1 40) = 40C1 ()  <br>

### Patch 14.24
"Geometric Random Variable" (Independent Trial) <br>
P(n) is a probability of success for the first time in n trial <br>
P(n) = pᵏ(1-p)ⁿ⁻¹ <br>
P(1) = (1/40)¹(39/40)⁰ <br>
P(2) = (1/40)¹(39/40)¹ <br>
P(3) = (1/40)¹(39/40)² <br>
P(4) = (1/40)¹(39/40)³ <br>
P(5) = (1/40)¹(39/40)⁴ <br>


## Result from Simulation


## Conclusion


## Source
<a href="https://teamfighttactics.leagueoflegends.com/en-sg/news/game-updates/teamfight-tactics-patch-14-23-notes/" target="_blank">Teamfight Tactics patch 14.23 notes</a>
<br>

<a href="https://teamfighttactics.leagueoflegends.com/en-ph/news/game-updates/teamfight-tactics-patch-14-24-notes/" target="_blank">Teamfight Tactics patch 14.24 notes</a>
<br>
