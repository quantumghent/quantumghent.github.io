---
title: "A tensor network approach to higher dimensional lattice gauge theories"
promoter: Frank Verstraete
supervisor: Lander Burgelman
contact: Lander Burgelman
topic: "Computational Quantum Many-Body Physics"
year: "2023"
---

#### Context

The concept of gauge symmetries is ubiquitous in many-body physics. Most notably, it underpins the Standard Model of elementary particle physics where the fundamental interactions of nature arise from the gauging of global symmetries, but gauge theories also appear in the context of low-temperature condensed matter systems. For small coupling regimes they can be studied using perturbation theory, giving rise to the well-known Feynman diagrammatic approach to quantum field theories which has led to results with an unrivaled precision. In contrast, this perturbative approach breaks down entirely when interactions become strong. Most notably, this is the case for the theory of quantum chromodynamics (QCD) which describes the strong interaction, where all low energy features are essentially non-perturbative.

Currently, the most accurate description of the strongly coupled behavior of gauge theories stems from a discrete formulation in terms of lattice gauge theory [1]. Over the past decades lattice QCD computations based on Monte Carlo sampling have reached impressive accuracy, for instance in the ab initio determination of the light hadron masses. In spite of these remarkable results, lattice Monte Carlo sampling suffers from some significant drawbacks. Most notably, it does not allow for real-time simulations of dynamical non-equilibrium phenomena, and cannot be used to study of systems with finite fermion densities.

Tensor network states form a variational class of wavefunctions that have proven extremely useful for describing low-energy physics of strongly correlated quantum many body systems. They constitute a non-perturbative approach to Hamiltonian systems, support finite fermion densities and allow simulation of real-time dynamics. In recent years there have been successful applications of this framework to 1+1 dimensional lattice gauge theories from a numerical perspective [2], while also leading to a deeper understanding of gauge invariance at the level of the quantum state itself [3]. The combination of recent advances in both the understanding of symmetries in quantum states and the development of variational tensor-network algorithms in our group [4] could pave the way to more ambitious simulations of lattices gauge theories in higher dimensions. This forms the topic of this master's thesis.

#### Goal

The goal of this thesis project is to gain a deeper understanding of gauge invariance at the level of quantum states, as well as using these insights for simulating lattice gauge theories. As a first step towards this goal, the student would familiarize themselves with the framework of lattice gauge theory and the characterization of gauge invariance of quantum states in terms of tensor networks. Expanding upon this from the theoretical side, the student could explore the relation between symmetries and their gauging in lattice models to tensor network realizations of higher-form symmetries and dualities. More concretely, a numerical aspect to the project would be to combine the established theoretical framework with novel variational methods developed in the group to tackle the simulation of higher dimensional lattice gauge theories. Finally, there could also be an additional technological aspect to considering lattice gauge theories from this angle. Just as insights from the use of quantum simulators have recently been adapted to tensor network studies, the concepts and algorithms studied in this thesis could in turn be investigated in a quantum hardware context.

[1] John B. Kogut. An introduction to lattice gauge theory and spin systems. [Reviews of Modern Physics 51, 659](https://doi.org/10.1103/RevModPhys.51.659) (1979)

[2] Boye Buyens, Jutho Haegeman, Karel Van Acoleyen, Henri Verschelde, and Frank Verstraete. Matrix Product States for Gauge Field Theories. [Physical Review Letters 113, 091601](https://arxiv.org/abs/1312.6654) (2013)

[3] Jutho Haegeman, Karel Van Acoleyen, Norbert Schuch, J. Ignacio Cirac, and Frank Verstraete. Gauging Quantum States: From Global to Local Symmetries in Many-Body Systems. [Physical Review X 5, 011024](https://arxiv.org/abs/1407.1025) (2015)

[4] [quantumghent.github.io/software](https://quantumghent.github.io/software)
