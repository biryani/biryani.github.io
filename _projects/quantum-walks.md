---
layout: project
title: Quantum walks and spatial search
description: Discrete-time quantum walk algorithms for search on graphs, and the stubborn two-dimensional case.
img: assets/img/projects/quantum-walks.svg
importance: 4
related_publications: true
---

Spatial search asks for a marked vertex on a graph when moves are restricted to edges — a constraint that makes Grover's algorithm inapplicable and quantum walks the natural tool. The difficulty concentrates in low dimensions: on a two-dimensional lattice the walk barely outruns classical search, and the gap between the achievable runtime and the conjectured optimum stayed open for a long time.

Most analyses assume a single marked vertex, which is not the typical case. Using a flip-flop quantum walk, search with multiple targets can be handled directly, and the resulting algorithm behaves predictably as the number and arrangement of targets vary {% cite abhijith2018spatial %}. Building on the same framework, the query complexity of spatial search in two dimensions can be improved — narrowing the margin in exactly the regime where quantum walks are weakest {% cite abhijith2019improving %}.
