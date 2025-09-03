---
title: "Compact Knapsack: a Semidefinite Approach"
collection: talks
type: "Talk"
permalink: /talks/2024-11-20-SDPCompactKP
venue: "PGMO Days 2024"
date: 2024-11-20
location: "Palaiseau, France"
#slidesurl: 'http://hubertvilluendas.github.io/files/TalkPGMO2024.pdf'
---

Work in progress about the min-knapsack problem. [Slides](files/TalkPGMO2024.pdf)

The min-knapsack with compactness constraint problem (min-KCP) is a variant of the classical knapsack problem, introduced in [The min-Knapsack problem with compactness constraints and applications in statistics](https://www.sciencedirect.com/science/article/pii/S0377221723005593). Given items \\(i\in\left\lbrace 1,\dots,n\right\rbrace\\) with cost $\\(c_i\\) and weight \\(w_i\\), the goal is to select objects \\(S\subseteq\left\lbrace 1,\dots,n\right\rbrace\\) minimizing the cost of the selection, while ensuring that the total weight exceeds a given constant \\(q\\), in such way that the selection is <strong>compact</strong>: for a given \\(\Delta\in\mathbb{N}\\), the distance separating two consecutive selected objects \\(i,j\in S\\) must not exceed \\(\Delta\\).

This problem can easily be modeled as a \\(0,1\\)-integer linear program. In this work, we propose a semidefinite formulation of this problem, and explain how to strengthen the basic semidefinite relaxation in order to get better bounds. Finally, we will show how the semidefinite model compares with the classical known cuts for the knapsack problem, such as cover inequalities.