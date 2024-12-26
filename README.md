# TFT-Set-13-Anomaly-Study
Have you ever wonder how many time do we have to roll until we found the anomaly that we're looking for in TFT Set13? <br><br>
![TeamfightTactics_Set13_IntotheArcane_KeyVisual_Powder_Sevika_Vander_Vi](https://github.com/user-attachments/assets/cf9b3a1e-c547-4252-b89f-c8ebfa2e9658)


## Overview
In this experiment we gonna test both patch 14.23 and 14.24 <br><br>
The different between these patch anomaly system is <br>
Patch 14.23 : The anomaly that have already been roll are not gonna appear again in the pool <br>
Patch 14.24 : The anomaly that have already been roll might be able to appear again in the pool <br><br>
If we compare this to the Probability Patch 14.23 would be "Dependent Trail", and Patch 14.24 would be "Independent Trial". 
Patch 14.24 have some adjustment to a few anomaly but the amount of the anomaly in this patch are still the same.
Time of simulation is around 10 million time for getting close to the theoratical probability as much as possible. <br>
<br>


## Hypothesis
### Patch 14.23 (Dependent Trial)
P(n) is a probability of success for the first time at n trial after fail n-1 trail <br>
P(n) = (Fail₁)(Fail₂)(Fail₃)...(Failₙ₋₁)(Success) <br> 
P(1) = (1/60) = 1/60 = 0.01666 <br>
P(2) = (59/60)(1/59) = 1/60 = 0.01666 <br>
P(3) = (59/60)(58/59)(1/58) = 1/60 = 0.01666 <br>
P(4) = (59/60)(58/59)(57/58)(1/57) = 1/60 = 0.01666 <br>
P(5) = (59/60)(58/59)(57/58)(56/57)(1/56) = 1/60 = 0.01666 <br>
P(60) = (59/60)(58/59)(57/58)(56/57)(1/56)...(1/2)(1/1) = 1/60 = 0.01666 <br>
Running out of anomaly after 60 trail <br>

### Patch 14.24 (Independent Trial)
This scenerio we could apply "Geometric Random Variable" <br>
P(n) is a probability of success for the first time at n trial after fail n-1 trail <br>
P(n) = pᵏ(1-p)ⁿ⁻¹ <br>
P(1) = (1/60)¹(59/60)⁰ = 0.01639 <br>
P(2) = (1/60)¹(59/60)¹ = 0.01612 <br>
P(3) = (1/60)¹(59/60)² = 0.01585 <br>
P(4) = (1/60)¹(59/60)³ = 0.01558 <br>
P(5) = (1/60)¹(59/60)⁴ = 0.01532 <br>
P(60) = (1/60)¹(59/60)⁵⁹ = 0.00608 <br>
P(100) = (1/60)¹(59/60)⁹⁹ = 0.00310 <br>
P(200) = (1/60)¹(59/60)¹⁹⁹ = 0.00058 <br>
This patch anomaly will not running out <br><br>


## Result from Simulation
### Patch 14.23 (Dependent Trial)
![Screenshot 2024-12-26 133633](https://github.com/user-attachments/assets/1eb0b984-6dab-4ce6-a623-114caab2e263)

### Patch 14.24 (Independent Trial)
![Screenshot 2024-12-26 133553](https://github.com/user-attachments/assets/2aa86f92-2e7c-49f2-b24f-e2a647bb4d87)
<br><br>

## Conclusion
The "Experimental Probability" and "Theoratical Probability" are pretty close.

### Patch 14.23 
In this patch, the chance of getting the anomaly we’re looking for increase every trail because we’re selecting anomalies that we’re not looking for out of the pool. But if we look at the number of trails to get the anomaly, the chance is the same for every trial. <br>
The expected value of this patch from simulation is around 30 so it mean we most likely to get anomaly that we're looking for in trial 30, in that case we need a spare gold around 60 gold to get anomaly that we're looking for.

### Patch 14.24 
In this patch, the chance of getting the anomaly we’re looking for is the same for every trial because we’re not selecting anomalies that we’re not looking for out of the pool. But if we look at the number of trails, the chance of getting the anomaly decreases the more trails we make. <br>
The expected value of this patch from simulation is around 60 so it mean we most likely to get anomaly that we're looking for in trial 60, in that case we need a spare gold around 120 gold to get anomaly that we're looking for.
<br><br>

## Source
<a href="https://teamfighttactics.leagueoflegends.com/en-sg/news/game-updates/teamfight-tactics-patch-14-23-notes/">Teamfight Tactics patch 14.23 notes</a>
<br>

<a href="https://teamfighttactics.leagueoflegends.com/en-ph/news/game-updates/teamfight-tactics-patch-14-24-notes/">Teamfight Tactics patch 14.24 notes</a>
<br>

<a href="https://youtu.be/h6QdOe8kUDM?si=xlZhD0uz-pEDYvyN">What's NEW in the 5 Week Patch | TFT Patch 14.24 Review</a>
<br>

<a href="https://youtu.be/WJQswHGe5sU?si=S3EnpCjzm_eOXJZ_">Patch 14.24 Preview and Anomalies Breakdown Part 2 - Set 13 Into the Arcane</a>
<br>
