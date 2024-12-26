# TFT-Set-13-Anomaly-Study
Have you ever wonder how many time do we have to roll until we found the anomaly that we're looking for in TFT Set13? <br><br>
![TeamfightTactics_Set13_IntotheArcane_KeyVisual_Powder_Sevika_Vander_Vi](https://github.com/user-attachments/assets/cf9b3a1e-c547-4252-b89f-c8ebfa2e9658)


## Overview
In this experiment we gonna test both patch 14.23 and 14.24 <br>
The different between these patch anomaly system is <br>
Patch 14.23 : The anomaly that have already been roll are not gonna appear again in the pool <br>
Patch 14.24 : The anomaly that have already been roll might be able to appear again in the pool <br>
If we compare this to the Probability Patch 14.23 would be "Dependent Trail", and Patch 14.24 would be "Independent Trial" <br>
Time of simulation is around 10 million time for getting close to the theoratical probability as much as possible <br>
<br>


## Hypothesis
### Patch 14.23 (Dependent Trial)
P(n) is a probability of success for the first time at n trial after fail n-1 trail <br>
P(n) = (Fail₁)(Fail₂)(Fail₃)...(Failₙ₋₁)(Success) <br> 
P(1) = (1/60) = 1/60 <br>
P(2) = (59/60)(1/59) = 1/60 <br>
P(3) = (59/60)(58/59)(1/58) = 1/60 <br>
P(4) = (59/60)(58/59)(57/58)(1/57) = 1/60 <br>
P(5) = (59/60)(58/59)(57/58)(56/57)(1/56) = 1/60 <br>
P(60) = (59/60)(58/59)(57/58)(56/57)(1/56)...(1/2)(1/1) = 1/60 <br>
Running out of anomaly after 60 trail <br>
Probability of getting anomaly that we are looking for after reroll n time is the same at every n attemp<br>

### Patch 14.24 (Independent Trial)
This scenerio we could apply "Geometric Random Variable" <br>
P(n) is a probability of success for the first time at n trial after fail n-1 trail <br>
P(n) = pᵏ(1-p)ⁿ⁻¹ <br>
P(1) = (1/40)¹(39/40)⁰ = 0.02500 <br>
P(2) = (1/40)¹(39/40)¹ = 0.02438 <br>
P(3) = (1/40)¹(39/40)² = 0.02377 <br>
P(4) = (1/40)¹(39/40)³ = 0.02317 <br>
P(5) = (1/40)¹(39/40)⁴ = 0.02259 <br>
P(60) = (1/40)¹(39/40)⁵⁹ = 0.00547 <br>
P(100) = (1/40)¹(39/40)⁹⁹ = 0.00199 <br>
P(200) = (1/40)¹(39/40)¹⁹⁹ = 0.00016 <br>
This patch anomaly will running out you might get the same in worse case you might find your anomaly at infinite trial <br>
Probability of getting anomaly that we are looking for in higher trail is lower than lower trial <br>


## Result from Simulation



## Conclusion



## Source
<a href="https://teamfighttactics.leagueoflegends.com/en-sg/news/game-updates/teamfight-tactics-patch-14-23-notes/">Teamfight Tactics patch 14.23 notes</a>
<br>

<a href="https://teamfighttactics.leagueoflegends.com/en-ph/news/game-updates/teamfight-tactics-patch-14-24-notes/">Teamfight Tactics patch 14.24 notes</a>
<br>
