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
{% comment %}
  Généré automatiquement depuis _talks/ :
  - les fiches sont regroupées par `topic` (à défaut : par `title`), sujet le plus récent en premier ;
  - si une fiche a une liste `presentations`, chaque entrée devient une ligne ;
    sinon la fiche donne une seule ligne (venue, location, date, slides).
{% endcomment %}
{% assign talks_by_topic = site.talks | sort: "date" | reverse | group_by_exp: "talk", "talk.topic | default: talk.title" %}
<ul>
{%- for group in talks_by_topic %}
  <li><strong>{{ group.name }}</strong>
    <ul>
    {%- assign topic_talks = group.items | reverse %}
    {%- for talk in topic_talks %}
      {%- if talk.presentations %}
        {%- assign presentations = talk.presentations %}
      {%- else %}
        {%- assign presentations = "" | split: "" | push: talk %}
      {%- endif %}
      {%- for p in presentations %}
        {%- assign kind = p.type | default: talk.type %}
      <li>{{ p.venue }} – {{ p.location }}, {{ p.date | date: "%B %Y" }}{% if kind == "Poster" %} – poster{% endif %}{% if p.slides %} (<a href="{{ base_path }}{{ p.slides }}">{% if kind == "Poster" %}poster{% else %}slides{% endif %}</a>){% endif %}</li>
      {%- endfor %}
    {%- endfor %}
    </ul>
  </li>
{%- endfor %}
</ul>

Supervision
======
* Master 1 MoSIG internship – <strong>Julia wrapper for BiqCrunch</strong>, a semidefinite-based solver for binary quadratic problems
  * Student: Gustavo Prolla Lacroix (Université Grenoble Alpes)
  * Co-supervised with Mathieu Besançon (LIG)
  * March–July 2026

Enseignement
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>