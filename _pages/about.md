---
permalink: /
title: "Présentation"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Je m'appelle Hubert Villuendas et je suis doctorant en mathématiques appliquées au sein du [Laboratoire Jean Kuntzmann](https://www-ljk.imag.fr/) et du [Laboratoire d'Informatique de Grenoble](https://www.liglab.fr/fr), sous la direction de Jérôme Malick et Mathieu Besançon.

Ma thèse porte sur les <strong>méthodes et applications de l'optimisation conique, mixte en nombre entiers</strong>. Plus précisément, l'optimisation conique en nombres mixtes (MICO) est une classe de problèmes d'optimisation où des variables de décision prennent des valeurs entières et des contraintes peuvent s'exprimer comme l'appartenance à un cône convexe \\(\mathcal{K}\subseteq\mathbb{R}^m\\) :

$$
\left[\begin{array}{rll}
\text{minimize} & c^\top x &\\
\text{subject to} & Ax-b\in \mathcal{K} &\\
& x_i\in\mathbb{Z} & \forall i\in\mathcal{I}
\end{array}\right.
$$

où \\(\mathcal{I}\subseteq\left\lbrace 1,\dots,n\right\rbrace\\), \\(A\in\mathbb{R}^{n\times m}\\) et \\(b\in\mathbb{R}^m\\).

L'optimisation conique généralise l'optimisation linéaire en introduisant des non-linéarités structurées qui capture un grand nombre de problèmes essentiels en <strong>recherche opérationnelle</strong>, <strong>optimisation combinatoire</strong>, ou encore en <strong >science des données</strong>.