---
title: "First-Order Methods for Distributionally Robust Mixed-Integer Optimization"
collection: talks
type: "Talk"
permalink: /talks/MixedIntegerFirstOrderWDRO
venue: "ROADEF 2026"
date: 2026-02-26
location: "Tours, France"
#slidesurl: 'http://hubertvilluendas.github.io/files/TalkROADEF2026.pdf'
---

Presentation about a Frank-Wolfe approach for Wasserstein distributionally robust optimization for combinatorial problems, also presented on *February 10, 2026* at *AIRO Young Workshop, Padova, Italy*. [Slides](/files/TalkROADEF2026.pdf)

We consider a general class of combinatorial optimization problems in which some imput data are only partly observed or subject to estimation errors. The problem can be written as a function of a scenario \\(\xi\in\Xi\\):

\\(\underset{z\in\mathcal{Z}}{\text{minimize}}\quad f(z,\xi),\\)

where \\(\mathcal{Z}\\) is the mixed-integer set of decision variables and \\(f(z,\xi)\\) is the optimal value of the combinatorial problem under scenario \\(\xi\\) for \\(\Xi\subseteq\mathbb{R}^d\\) the set of all possible scenarios of the uncertain data. For example, in a facility location problem with uncertain demand, \\(\mathcal{Z}\\) would be the set of facility opening vectors and \\(f(z,\xi)\\) the optimal value for the opening \\(z\\) under demand \\(\xi\\), which can itself be a convex program.

Assuming that the data follows an unknown probability distribution \\(\mathbb{P}\\), the ideal goal is to choose \\(z\\) to minimize the expected value \\({\mathbb{E}}[f(z,\cdot)]\\). When the probability distribution of uncertain parameters is unknown, one typically relies on a finite historical dataset \\(\lbrace\widehat{\xi}_1,\dots,\widehat{\xi}_N\rbrace\subset\Xi\\) to infer plausible distributions. Using the empirical measure \(\widehat{\mathbb{P}}_N\\), data driven models typically relies on empirical risk minimization

\\(\min_{z\in\mathcal{Z}}\dfrac{1}{N}\displaystyle\sum^N_{i=1}f\left(z,\widehat{\xi}_i\right).\\)

However, this approach can fail in the case where \\(N\\) is small or when the deployment data differs from the training data. In this context, Wasserstein Distributionally Robust Optimization (WDRO) has become a powerful framework, by its nice modeling and generalisation properties [[Esfahani and Kuhn, 2018](https://link.springer.com/content/pdf/10.1007/s10107-017-1172-1.pdf), [Le and Malick, 2024](https://arxiv.org/pdf/2402.11981), [Wiesemann, 2014](https://optimization-online.org/wp-content/uploads/2013/02/3757.pdf)]: we minimize the expected value of \\(f(z,\cdot)\\) under the worst-case distribution within a neighborhood of the empirical measure \\(\widehat{\mathbb{P}}_N\\). This leads to the problem:

\\(\min_{z\in\mathcal{Z}} \sup_{\mathbb{Q}\in\mathrm{Proba}\left(\Xi\times\Xi\right)}\mathbb{E}_{\zeta\sim\mathbb{Q}}\left[f(,\zeta)\right]\\)

where \\(W_c(\cdot,\cdot)\\) denotes the Wasserstein distance [[Cuturi and Peyré](https://arxiv.org/pdf/1803.00567)]. Instead of (WDRO), we propose to use its entropic-regularized version, following [[Azizian, Iutzeler and Malick, 2023](https://www.esaim-cocv.org/articles/cocv/pdf/2023/01/cocv220004.pdf)]. This problem retains the generalization and robustness guarantees of the original formulation and enables the computation of stochastic gradient estimators via a Monte-Carlo sampling method [[Vincent et al, 2024](https://arxiv.org/pdf/2410.21231)]. 

Then, we use a stochastic Frank-Wolfe algorithm to handle sampling noise [[Braun et al, 2025](https://arxiv.org/pdf/2211.14103)] which preserves the combinatorial nature of the feasible set while ensuring scalability. Our approach is close to oracle-based methods for robust optimization and is complementarty to existing WDRO approaches for mixed-integer problems that rely on exact reformulations combined with branch-and-bound or cutting-plane methods. Our use of a stochastic Frank--Wolfe algorithm enables an oracle-based optimization over \\(\mathrm{conv}(\mathcal{Z})\\), avoiding an explicit description of the feasible set and allowing efficient treatment of rich combinatorial structures.

This framework thus extends the applicability of WDRO methods to mixed-integer and discrete optimization problems, offering a principled and computationally efficient approach to decision-making under uncertain data. 