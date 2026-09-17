---
layout: project
title: Quantum algorithms and applications
description: What quantum computers can actually do for concrete problems — and where the claims break down.
img: assets/img/projects/quantum-algorithms.svg
importance: 3
papers:
  - abhijith2022quantum
  - bartschi2024potential
  - shastry2022reliable
  - pareek2025limitations
---

The gap between an asymptotic speedup on paper and a useful result on a real machine is where most quantum-advantage claims fail. This work sits in that gap: implementing algorithms concretely enough to see their real cost, surveying where the plausible applications actually are, and stating plainly when the accounting does not work out.

The implementation side began as a survey of quantum algorithms written at the level of actual circuits rather than oracle queries, covering a broad range of standard algorithms in enough detail to run them. Mapping the application space more broadly — across simulation, optimization, and machine learning — sets out where quantum computing is most likely to pay off in a national-laboratory research portfolio.

Within machine learning, quantum kernel methods are a leading candidate application, but their cost is dominated by circuit evaluations. Reducing the number of evaluations needed for reliable classification attacks the bottleneck directly. The negative results matter just as much. Quantum linear system solvers are frequently invoked as the engine behind proposed speedups for power-flow problems; examined closely, even fault-tolerant solvers do not deliver the claimed advantage for quantum power flow, because the input and readout costs dominate the solve.
