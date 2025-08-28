---
title: "Compact Knapsack: a Semidefinite Approach"
collection: talks
type: "Talk"
permalink: /talks/2025-11-20-SDPCompactKP
venue: "ROADEF 2025"
date: 2025-02-26
location: "Marne-la-vallée, France"
---

Presentation about the min-knapsack problem.

The min-knapsack with compactness constraint problem (min-KCP) is a variant of the classical knapsack problem, introduced in [The min-Knapsack problem with compactness constraints and applications in statistics](https://www.sciencedirect.com/science/article/pii/S0377221723005593), originally to solve the problem of detecting regime changes in time series. Given items \\(i\in \left\lbrace 1,\dots,\right\rbrace\\) with cost \\(c_i\\) and weight \\(w_i\\), the goal is to select objects \\(S\subseteq\left\lbrace 1,\dots,n\right\rbrace\\) minimizing the cost of the selection, while ensuring that the total weight exceeds a given constant \\(q\\), in such way that the selection is <strong style="color: #197ac9;">compact</strong>: for a given \\(\Delta\in\mathbb{N}\\), the distance separating two consecutive selected objects \\(i,j\in S\\) must not exceed \\(\Delta\\). 

In this work, we propose a semidefinite reformulation of this problem, and explain how to strengthen the baseline semidefinite relaxation in order to get better bounds, and show how the semidefinite model compares with the classical known cuts for the knapsack problem, such as cover inequalities.

A second part of the work focuses on the efficiency of penalized versions of the semidefinite relaxation and how this approach can effectively address the original statistical problem.