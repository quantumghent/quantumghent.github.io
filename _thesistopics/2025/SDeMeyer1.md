---
title: "How high is high enough. Finite-Temperature analysis of the Hubbard model to computationally probe high-temperature superconductivity"
promoter: Jutho Haegeman
supervisor: Sander De Meyer
contact: Sander De Meyer
topic: "Computational Quantum Many-Body Physics"
year: "2025"
---

#### Context

High-temperature superconductivity was first discovered in 1986 when a system of barium, lanthanum, copper, and oxide exhibited a critical temperature of 30K—then the highest recorded. However, BCS theory, the original framework for superconductivity, failed to explain this phenomenon.  A complete theory of this effect is still missing, more than 40 years after its discovery.

To study and simulate superconductivity, the Hubbard model was introduced as a minimal model. It describes fermions hopping on a (in the case of the cuprates: square) lattice, with a hopping term and a repulsive term [1]

$$H = -t \sum_{<i j> \sigma} \left(\hat{c}_{i \sigma}^\dagger \hat{c}_{j \sigma} + h.c.\right) + U \sum_i \hat{n}_i \hat{n}_j$$.


However, solving it remains a significant challenge, leading to the development of numerous computational approaches. Among these, Tensor Networks (TN) have emerged as a powerful tool, explicitly capturing strong correlations without suffering from the sign problem  (like Quantum Monte Carlo methods). In particular, the two-dimensional TN variant, Projected Entangled-Pair States (PEPS), is widely used but has been primarily applied to ground-state (0K) calculations and static properties. To get more insight into the Hubbard model, it is crucial to extend these methods to finite-temperature states and their time evolution [2].

A key computational challenge in the latter is evaluating the exponential of the Hamiltonian. For finite temperatures, this requires computing the density operator:

$$\rho(\beta) = e^{-\beta H}$$
 
Since this is exponentially hard in the system size, approximations are necessary. The traditional approach relies on the Suzuki-Trotter decomposition, but a more recent and accurate alternative is to use cluster expansions (see Figure 1) [3,4].

<p><img alt="Fig. 1: Example of cluster expansions" src="/images/thesistopics/2025/SDeMeyer1.png" style="float:right; width:300px" /></p>

#### Goal

This thesis will explore different methods for probing the finite-temperature phase diagram of the Hubbard model. There are multiple directions that could be taken depending on the interests of the student. One possibility is implementing a new algorithm based on the Suzuki-Trotter decomposition and comparing it with the existing cluster expansion code, or by using the purification instead of the thermal density operator [5]. Another is using cluster expansions to study various parameter regimes of the Hubbard model, looking both at the feasibility and computational cost of obtaining accurate results. Further optimizations to enhance efficiency may also be considered. These methods will allow us to look at the finite-temperature phase diagram of the Hubbard model (see Figure 2).

<p><img alt="Fig. 2: Phase diagram of the Hubbard model" src="/images/thesistopics/2025/SDeMeyer2.png" style="float:right; width:300px" /></p>

[1] Qin M. (2021) [arxiv:2104.00064](https://arxiv.org/abs/2104.00064)

[2] Sinha A. (2022) [arxiv:2209.00985](https://arxiv.org/pdf/2209.00985)

[3] Vanhecke B. (2021) [arxiv:2112.01507](https://arxiv.org/abs/2112.01507)

[4] Vanhecke B. (2019) [arxiv:1912.10512](https://arxiv.org/abs/1912.10512)

[5] Czarnik P. (2018) [arxiv:1811.05497](https://arxiv.org/abs/1811.05497)
