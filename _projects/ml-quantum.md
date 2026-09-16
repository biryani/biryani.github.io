---
layout: project
title: Machine learning for quantum systems
description: Statistical estimation applied to quantum states and the devices that realize them.
img: assets/img/projects/ml-quantum.jpg
importance: 2
related_publications: true
---

Characterizing a quantum system from measurements is an estimation problem, and a badly conditioned one: the state space grows exponentially, the measurements are noisy, and the noise is entangled with the thing being measured. This work brings learning-theoretic tools to bear on that problem, at both the level of abstract states and the level of real hardware.

For many-body states, the question is representation. Energy-based models give a compact parameterization of quantum many-body states that can be fit from data rather than constructed analytically, which makes previously inaccessible states tractable to describe {% cite PhysRevResearch.6.033201 %}. The same pressure toward sample efficiency drives the treatment of lattice gauge theories with fermions, where each configuration is expensive to produce {% cite xlz6-yzxc %}.

On hardware, the central difficulty is that state-preparation and measurement (SPAM) errors are confounded with the state itself — standard tomography attributes device error to the state and vice versa. Estimating both simultaneously, in a single framework that does not privilege one over the other, resolves the confound {% cite Jayakumar2024universalframework %}. Analog devices raise a sharper version of the same problem, since there is no gate decomposition to fall back on: what the machine actually implements has to be learned directly. Recovering the response functions of neutral-atom and superconducting platforms turns that calibration into an inference problem {% cite tuysuz2025learning %}.
