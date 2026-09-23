---
title: "First-Order Methods for Wasserstein Distributionally Robust Constrained Optimization"
collection: publications
category: manuscripts
permalink: /publication/2026-First-Order_Methods_for_WDRO_Constrained_Problems
excerpt: 'We consider constrained problems in which input data are affected by errors. In such settings, Wasserstein distributionally robust optimization provides a principled framework to mitigate model risk by optimizing against worst-case data distributions within Wasserstein ambiguity sets.
However, the numerical resolution of the resulting problems remains challenging, especially in constrained settings.
In this paper, we provide a general, practical way to solve Wasserstein distributionally robust formulations in the presence of constraints. 
Our approach only requires a linear minimization oracle for the feasible set, and combines two key ingredients: (i) an entropic regularization of the distributionally robust value function, which makes it possible to compute stochastic gradient estimators, and (ii) a stochastic Frank-Wolfe algorithm, which minimizes the regularized robust objective while naturally handling constraints.
We illustrate the method, its tractability, and its interests against empirical risk minimization, on two operations research problems: the traffic assignment and the minimum quadratic spanning tree.'
date: 2026-09-19
venue: 'Preprint arXiv'
paperurl: 'http://hubertvilluendas.github.io/files/FirstOrderWDROforConstraindPbm.pdf'
citation: 'Hubert Villuendas, Mathieu Besançon and Jérôme Malick. (2026). &quot;First-Order Methods for Wasserstein Distributionally Robust Constrained Optimization.&quot; <i>preprint arXiv:2607.11460</i>.'
---

We consider constrained problems in which input data are affected by errors. In such settings, Wasserstein distributionally robust optimization provides a principled framework to mitigate model risk by optimizing against worst-case data distributions within Wasserstein ambiguity sets.
However, the numerical resolution of the resulting problems remains challenging, especially in constrained settings.
In this paper, we provide a general, practical way to solve Wasserstein distributionally robust formulations in the presence of constraints. 
Our approach only requires a linear minimization oracle for the feasible set, and combines two key ingredients: (i) an entropic regularization of the distributionally robust value function, which makes it possible to compute stochastic gradient estimators, and (ii) a stochastic Frank-Wolfe algorithm, which minimizes the regularized robust objective while naturally handling constraints.
We illustrate the method, its tractability, and its benefits over empirical risk minimization, on two operations research problems: the traffic assignment and the minimum quadratic spanning tree.
