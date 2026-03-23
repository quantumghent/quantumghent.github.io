---
title: "From Microscopic Disorder to Universal Physics: A Tensor Network Study of Random Spin Chains"
promoter: Nick Bultinck
supervisor: Kevin Vervoort, Wei Tang
contact: Kevin Vervoort
topic: "Condensed Matter Physics"
year: "2026"
---

#### Context

Classifying and understanding phases of quantum many-body systems is one of the central goals of modern condensed matter physics. While clean, translationally invariant systems have been studied extensively and are often well understood, real-world materials inevitably contain disorder. Randomness in microscopic couplings can fundamentally alter low-energy physics, giving rise to new universality classes, unconventional critical points, and exotic phases such as infinite-randomness fixed points and Griffiths phases.

Random spin chains provide a paradigmatic setting in which disorder plays a decisive role. A celebrated example is the random Heisenberg or transverse-field Ising chain, where renormalisation group [1] approaches reveal that disorder can drive the system toward strong-disorder fixed points with activated dynamical scaling and broad distributions of observables. In these systems, universal behaviour emerges not despite, but because of, the flow toward increasingly broad coupling distributions under renormalisation.

However, an important conceptual and practical question remains only partially understood: to what extent do microscopic details of the disorder distribution affect universal behaviour and observable quantities in finite systems? While universality suggests insensitivity to short-distance details, numerical simulations necessarily probe finite-size systems and finite disorder realisations. In this regime, properties such as the shape of the coupling distribution (e.g. Gaussian, box, power-law, log-normal), its tails, and correlations between couplings may strongly influence convergence, entanglement growth, and numerical stability.

Tensor network methods [2], in particular matrix product states (MPS) and related algorithms, provide one of the most powerful numerical frameworks to study one-dimensional quantum systems. They allow efficient representation of low-entanglement states and enable precise computations of ground-state properties, entanglement entropies, correlation functions, and dynamical observables. Recently developed tensor network techniques for disordered systems by our group [1],  significantly enhance our ability to simulate random spin chains at large system sizes and for broad disorder regimes.

These advances open the possibility to systematically investigate how microscopic disorder distributions influence both (i) the emergent universal behaviour of random spin chains and (ii) the numerical performance and stability of tensor network algorithms themselves.

References:

[1] [M. Fisher, Phys. Rev. B 40, 546](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.51.6411)

[2] [J. I. Cirac, D. Pérez-García, N. Schuch, F. Verstraete, arXiv:2011.12127](https://arxiv.org/abs/2011.12127)

[3] [K. Vervoort, W. Tang, N. Bultinck, arXiv:2504.21089](https://arxiv.org/abs/2504.21089)

#### Goal

This project will investigate random quantum spin chains using tensor network techniques, with a particular focus on the interplay between microscopic disorder distributions, universal low-energy behaviour, and numerical performance.

First, the student will familiarize themselves with our extensive numerical toolbox. In addition the student will explore the existing literature about renormalisation group approaches to disordered systems (e.g. strong-disorder RG) and tensor network methods for one-dimensional quantum systems.

Second, the student will implement and benchmark tensor network simulations of prototypical random spin chains (e.g. random Heisenberg or transverse-field Ising models). Different classes of disorder distributions will be systematically explored, and their effect on physical properties like entanglement entropy scaling, correlation functions and effective critical exponents, ... . In addition the effect of the distributions on the convergence and stability of the numerical methods will be studied.

The project will be carried out in an international research environment. This project is well-suited for students with a keen interest in quantum physics and numerical simulations.
