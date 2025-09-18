---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

Academic Background
======
* PhD in Applied Mathematics – <strong>Methods and applications of mixed integer conic optimisation</strong>
  * Université Grenoble Alpes, Laboratoire Jean Kuntzmann (LJK) & Laboratoire d'Informatique de Grenoble (LIG)
  * Co-supervised by Jérôme Malick (LJK) and Mathieu Besançon (LIG)
  * Since 2023

* Master 2 ORCO (Operations Research, Combinatorics and Optimization)
  * Université Grenoble Alpes, IM²AG
  * 2023–2024
  * Internship: <strong>Mixed-Integer Conic Optimization for Combinatorial Problems</strong> (supervised by Mathieu Besançon, LIG)

* Master in Fundamental Mathematics – Research in Number Theory and Algebraic Geometry 
  * Université Grenoble Alpes, Institut Fourier
  * 2021–2023
  * Internships:
    * <strong>Higher trace forms of separable algebras</strong> (supervised by Grégory Berhuy, M2)
    * <strong>Simple group of order 168</strong> (supervised by Grégory Berhuy, M1)

* Magistère in Mathematics and Applications
  * Université Grenoble Alpes, Institut Fourier
  * 2020–2023
  * Research Internship: <strong>Algebras of finite representation type</strong> (supervised by Claire Amiot)

Articles
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

Enseignement
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>