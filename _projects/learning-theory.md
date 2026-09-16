---
layout: project
title: Learning theory for exponential families
description: Provable, sample-efficient recovery of high-dimensional discrete distributions.
img: assets/img/projects/learning-theory.svg
importance: 1
related_publications: true
---

Exponential-family distributions over discrete variables — Ising models, Potts models, general graphical models — are the workhorse description of correlated high-dimensional data, but fitting them is hard: the partition function is intractable, and the natural estimators trade tractability for statistical guarantees that are difficult to pin down. The line of work here asks what can be recovered, from how many samples, and under what assumptions on where those samples came from.

The starting point was structure learning with neural networks, which showed that a parameterized estimator could recover discrete graphical models without paying the usual price in sample complexity {% cite jayakumar2020learning %}. A persistent gap in that literature is the assumption that samples are drawn at equilibrium — rarely true of real physical or simulated systems, which are routinely observed in long-lived metastable states. Relaxing that assumption turns out not to be fatal: discrete distributions remain learnable from metastable samples, with guarantees that survive the departure from equilibrium {% cite jayakumar2026discrete %}.

Score matching sidesteps the partition function entirely and is widely used, but its finite-sample behavior was understood far less sharply than its asymptotics. Establishing finite-sample bounds puts the estimator on the same footing as the alternatives and makes the tradeoff against them explicit {% cite smedira2026finite %}. The same machinery carries into physics: lattice gauge theories with fermions are exactly the regime where sample-efficient learning matters most, since generating configurations is the dominant cost {% cite xlz6-yzxc %}.
