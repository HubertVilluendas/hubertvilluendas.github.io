---
title: "Mathematics for Computer Science (TD)"
collection: teaching
type: "M1 MoSIG"
permalink: /teaching/2025-maths4computerscience
venue: "Université Grenoble Alpes"
date: 2025-09-01
location: "Grenoble, France"
---

The aim of this course is to provide the necessary foundations for each student to be able to use the appropriate mathematical tools to develop well-founded reasoning and prove properties. It provides an overview of demonstration techniques, recurrence, bijections and algorithms, the basics of enumeration and combinatorics, divisibility, discrete structures and graphs, probabilities, modelling of classical laws, and random walks.

Ressources
======

- **TD1** [Correction TD1](/files/Maths4ComputerScience - Correction TD1.pdf)
    - [Sum of the cubes - visual proof 1](https://www.youtube.com/shorts/y4xi1a8sw-M?feature=share)
    - [Sum of the cubes - visual proof 2](https://www.youtube.com/shorts/dOCk6SSpWLo?feature=share)
    - [Sum of the cubes - visual proof 3](https://www.youtube.com/shorts/SZsMVGqUiic?t=7&feature=share)

- **TD2** [Correction TD2](/files/Maths4ComputerScience - Correction TD2.pdf)
    - [Explaination about *The Josephus Problem*](https://youtu.be/uCsD3ZGzMgE)

- **TD3** [Correction TD3](/files/Maths4ComputerScience - Correction TD3.pdf) 

- **TD4** [Correction TD4](/files/Maths4ComputerScience - Correction TD4.pdf)
    - [Video about Catalan Numbers *(in french)*](https://youtu.be/etzcN6g-vNY)
    - [Another one: Catalan Numbers *(in english)*](https://youtu.be/fczN0BCx0xs)

- **TD5** [Correction TD5](/files/Maths4ComputerScience - Correction TD5.pdf) 


Internship proposal
======
**Development of a Julia wrapper for the BiqCrunch solver (binary quadratic optimisation and semi-definite programming).**

- Co-supervised with Mathieu Besançon, hosted at the LIG (Laboratoire d'Informatique de Grenoble) at the GHOST team.

- *Context* : in the study of binary quadratic problems (BQP), positive semidefinite relaxations (SDPs) are commonly used to provide quality bounds. We model these problems in [Julia](https://julialang.org/) using [JuMP](https://jump.dev/), and currently solve them using solvers such as Mosek, SCS, Clarabel, *etc*. The [BiqCrunch](https://biqcrunch.lipn.univ-paris13.fr/) solver (implemented in C) is particularly well suited to BQP: it constructs efficient SDP relaxations to generate strong bounds, which are then exploited in a branch-and-bound approach.The proposed internship aims to develop a Julia wrapper to interface BiqCrunch with JuMP/MathOptInterface. If time permits, we will also consider creating a documented Julia package to facilitate the use of BiqCrunch within the JuMP community.

<!--Heading 2
======

Heading 3
====== -->
