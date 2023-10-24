---
title: Research
layout: default
permalink: /research/
---
## Research Interests
My research primarily focuses on the optimal control of systems that may have sudden, drastic changes at random times like a vehicle that may suddenly get a flat tire or an animal that may need to suddenly escape a predator in its environment.
I model these scenarios using piecewise-deterministic Markov processes (PDMPs), a special class of hybrid systems.
I focus on problems where the dynamics of the model depend on some ``operating mode'' that can change at random times (though with known rates).
Optimal control of the system then consists of finding input values that maximize or minimize a specified objective.
To do this, I employ techniques from dynamic programming and numerical methods for Hamilton-Jacobi-Bellman (HJB) equations.
Additionally, many of the projects listed below involve contributions from students in an REU where I served as a graduate student mentor.

## Ongoing work

### Navigating the Landscape of Fear
Joint work with Alexander Vladimirsky, Nicolas Gonzalez Granda, Sunay Joshi, Nagaprasad Rudrapatna, and Anne Somalwar.
The term “Landscape of Fear” broadly refers to the impact of predators (real or perceived) on the spatial distribution of and resource utilization by foraging prey animals. In this project, we extend ideas from classical optimal foraging theory continuous, two-dimensional spatial domain. We also seek to capture the impact of predation, imperfect planning, and the depletion of food on the optimal behavior of the planner. We model this system as a PDMP, where one mode corresponds to foraging and another corresponds to avoiding predators. Using the resulting optimal policies, we construct optimal trajectories and examine predicted usage patterns across various environments. This work was recently presented at SIAM-CT23 and was covered in [SIAM news](https://sinews.siam.org/Details-Page/foraging-behaviors-predation-risk-and-the-landscape-of-fear).
<!-- ### Optimal Control of Partially-Observed Predator-Prey Systems
Joint work with Alexander Vladimirsky, Steve Ellner, Suresh Sethi, and Kimberly Fitzpatrick -->

### Occassionally-Observed PDMPs
Joint work with Alexander Vladimirsky, Natasha Patnaik, and Nagaprasad Rudrapatna.  
What if we seek to control a system modelled by a PDMP, but we can only observe the operating mode at infrequent observation times? This project explores optimal path-planning for a variety of observation frequencies, including deterministic schedules, stochastic schedules, and observation times as a control variable. Additionally, we will explore a range of planning horizons such as finite horizon, infinite horizon, and exit-time problems.

## Selected Completed Projects

### Optimal Path Planning with Random Breakdowns
Joint work with Alexander Vladimirsky
Here we looked at optimal path-planning for an autonomous vehicle in a hazardous environment where there is a risk of breaking down. We identified three operating modes based on the vehicle's current level of functionality, and used this to come up with a PDMP model for the system. We generated optimal trajectories that minimize a general expected cost function that can be used to account for travel time, fuel costs, or other considerations. To generate numerical solutions, we relied on hybrid value-policy iterations, a method that combines value iterations and policy iterations to speed up convergence of value function computations. [Publication](https://doi.org/10.1109/LCSYS.2021.3130193).

### Pandemic Mitigation Strategies on Transportation Networks
Joint work with Samitha Samaranayake, Qi Luo, Benedetto Piccoli, and Daniel Work.
Public transportation is an area of high-transmission of infectious diseases. In this project, we looked at strategies to minimize the spread of COVID-19 in a transportation network through selective station closures. We used a generalized next generation matrix to identify stations that contributed most to the spread of disease along the network and proposed closure strategies based on these results. [Publication](https://doi.org/10.1016/j.trc.2022.103592).

### Modeling the Onset and Treatment of Type I Diabetes
Joint work with Lisette de Pillis, Blerta Shtylla, and An Do
This project looked at a compartment model of the onset of Type 1 diabetes and the impact of early treatment on the progression of the disease. We fit model parameters based on results in mouse models, performed sensitivity analysis for the system, and showed examples of when treatment is likely to be effective at slowing the development of the disease. [Publication](https://doi.org/10.3389/fphys.2019.01107).
