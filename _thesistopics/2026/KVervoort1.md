---
title: "The Good, The Bad and The Bose Glass"
promoter: Nick Bultinck
supervisor: Kevin Vervoort, Akshay Shankar, Wei Tang
contact: Kevin Vervoort
topic: "Condensed Matter Physics"
year: "2026"
---

#### Context

Understanding the interplay between interactions and disorder is a central problem in condensed matter physics. While clean one-dimensional bosonic systems are well described by Luttinger liquid theory and exhibit the well-known superfluid–Mott insulator transition, the presence of disorder fundamentally alters their behaviour. Even weak randomness can destabilise long-range coherence and generate new quantum phases that have no analogue in clean systems.

A paradigmatic model capturing this physics is the disordered Bose–Hubbard chain. In addition to the superfluid and Mott insulating phases, disorder induces the Bose glass phase, which is insulating yet gapless and compressible. Unlike conventional phases, the Bose glass is characterised by strong spatial inhomogeneity and the presence of rare regions that locally resemble different phases. As a result, its physical properties are governed by broad distributions of observables and rare fluctuations rather than uniform bulk behaviour.

Renormalisation group [1] approaches suggest that disorder-driven transitions in one dimension may be governed by strong-disorder fixed points with unconventional scaling properties. In these regimes, rare-region (Griffiths) effects play a dominant role, leading to anomalous dynamical behaviour and broad distributions of energy scales. Despite substantial theoretical work, several fundamental questions remain open. In particular, the precise nature of the superfluid–Bose glass transition is still debated, including the universality of its critical behaviour and the role played by rare regions. Understanding how these features manifest in physical observables such as correlation functions, entanglement properties, and dynamical response remains an active area of research. 

<p><img alt="Fig. 1: Phase diagram of the random Bose-Hubbard Chain." src="/images/thesistopics/2026/KVervoort1.png" style="float:right; width:350px" /></p>

Numerical simulations are essential for addressing these questions. One-dimensional systems are particularly well suited to tensor network methods [2], which provide efficient representations of weakly entangled quantum states. Matrix product state techniques enable accurate calculations of ground-state properties, correlations, and entanglement for system sizes far beyond exact diagonalisation. Recent algorithmic developments for disordered systems, such as those introduced in [3], further improve the stability and efficiency of tensor network simulations in strongly inhomogeneous settings.

References:

[1] [M. Fisher, Phys. Rev. B 40, 546](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.40.546)

[2] [J. I. Cirac, D. Pérez-García, N. Schuch, F. Verstraete, arXiv:2011.12127](https://arxiv.org/abs/2011.12127)

[3] [K. Vervoort, W. Tang, N. Bultinck, arXiv:2504.21089](https://arxiv.org/abs/2504.21089)

#### Goal

The goal of this project is to study disordered bosonic chains using tensor network methods, with a focus on the physics of the Bose glass phase and the critical behaviour of disorder-driven transitions.

The project will begin with a literature study introducing the theoretical framework of one-dimensional bosonic systems. The student will familiarise themselves with Luttinger liquid theory, the Bose–Hubbard model, and the superfluid–Mott insulator transition in clean systems. The effects of disorder will then be explored, including the emergence of the Bose glass phase, renormalisation group descriptions of disordered systems, and the role of rare-region physics in low-dimensional quantum matter. In parallel, the student will become acquainted with tensor network techniques for bosonic lattice models.

Building on this background, the student will use the extensive tensor network toolbox for simulations of disordered Bose–Hubbard chains and use them to investigate the properties of the different phases. Particular attention will be given to identifying signatures of superfluid, insulating, and glassy behaviour through correlation functions, compressibility, excitation gaps, and entanglement entropy. The transition between the superfluid and Bose glass phases will be studied in detail, with the aim of probing its scaling behaviour and identifying possible signatures of strong-disorder physics.

This project is well suited for students with a strong interest in theoretical and computational condensed matter physics. It combines concepts from quantum many-body theory, statistical mechanics of disordered systems, and modern numerical methods. No prior knowledge of tensor networks or disordered bosonic systems is required.
