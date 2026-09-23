---
permalink: /
title: "Presentation"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

My name is Hubert Villuendas and I am a PhD student in applied mathematics at the [Jean Kuntzmann Laboratory](https://www-ljk.imag.fr/) and the [Grenoble Computer Science Laboratory](https://www.liglab.fr/fr), under the supervision of [Jérôme Malick](https://membres-ljk.imag.fr/Jerome.Malick/) and [Mathieu Besançon](https://matbesancon.xyz/).

My thesis focuses on <strong>methods and applications of mixed-integer non-linear optimisation</strong>. More specifically, I focus on mixed-integer conic optimisation, where decision variables take integer values and constraints can be expressed as belonging to a convex cone \\(\mathcal{K}\subseteq\mathbb{R}^m\\):

$$
\left[\begin{array}{rll}
\text{minimize} & c^\top x &\\
\text{subject to} & Ax-b\in \mathcal{K} &\\
& x_i\in\mathbb{Z}^p\times\mathbb{R}^{n-p} & \forall i\in [\![n]\!]
\end{array}\right.
$$

where \\(A\in\mathbb{R}^{n\times m}\\) and \\(b\in\mathbb{R}^m\\).

Conic optimisation generalises linear optimisation by introducing structured non-linearities that capture a large number of essential problems in <strong>operational research</strong>, <strong>combinatorial optimisation</strong>, and <strong>data science</strong>.

My most recent research focuses on <strong>Distributionally Robust Optimization</strong> for <strong>data-driven constrained problems</strong>. Consider a mathematical program over a constrained feasible set \\(\mathcal{X}\\) with a non-linear stochastic objective \\(\mathbb{E}_{\xi\sim\mathbb{P}}[f(x,\xi)]\\), where the loss function \\(f\\) depends on an unknown random variable, a <strong>scenario</strong> \\(\xi\in\Xi\subseteq\mathbb{R}^d\\). Given training data \\(\widehat{\xi}_1,\dots,\widehat{\xi}_N\\), we build the empirical distribution \\(\widehat{\mathbb{P}}_N=(\delta_{\widehat{\xi}_1}+\dots+\delta_{\widehat{\xi}_N})/N\\) and we aim to find a feasible \\(x\in\mathcal{X}\\) that minimizes the objective under the worst possible distribution within a neighbourhood of the empirical distribution:

$$
\left[\begin{array}{rll}
\text{minimize} & \sup_{\substack{\mathbb{Q}\in\mathcal{M}^+(\Xi)\\ W_c(\mathbb{Q},\widehat{\mathbb{P}}_N)\leq\varrho}}\mathbb{E}_{\zeta\sim\mathbb{Q}}\left[f(x,\zeta)\right] &\\
\text{subject to} & x\in\mathcal{X}
\end{array}\right.
$$