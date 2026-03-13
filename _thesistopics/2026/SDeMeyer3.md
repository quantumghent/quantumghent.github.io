---
title: "2 hot 2 handle: Cooling down the Hubbard model to computationally probe high-temperature superconductivity"
promoter: Jutho Haegeman
supervisor: Sander De Meyer
contact: Sander De Meyer
topic: "Computational Quantum Many-Body Physics"
year: "2026"
---

#### Context

High-temperature superconductivity was first discovered in 1986 when a system of barium, lanthanum, copper, and oxide exhibited a critical temperature of 30K—then the highest recorded. However, BCS theory, the original framework for superconductivity, failed to explain this phenomenon.  A complete theory of this effect is still missing, more than 40 years after its discovery.

To study and simulate superconductivity, the Hubbard model was introduced as a minimal model. It describes fermions hopping on a (in the case of the cuprates: square) lattice, with a hopping term and a repulsive term [1]

$$ H = -t \sum_{<i j> \sigma} \left(\hat{c}_{i \sigma}^\dagger \hat{c}_{j \sigma} + h.c.\right) + U \sum_i \hat{n}_i \hat{n}_j $$.

<p><img alt="Fig. 1: Phase diagram of the Hubbard model" src="/images/thesistopics/2026/SDeMeyer3.png" style="float:right; width:350px" /></p>

However, solving it remains a significant challenge, leading to the development of numerous computational approaches. Among these, Tensor Networks (TN) have emerged as a powerful tool, explicitly capturing strong correlations without suffering from the sign problem (like Quantum Monte Carlo methods). In particular, the two-dimensional TN variant, Projected Entangled-Pair States (PEPS), is widely used but has been primarily applied to ground-state (0K) calculations and static properties. To get more insight into the Hubbard model, it is crucial to extend these methods to finite-temperature states and their time evolution [2]. This would allow us to accuretly predict the finite-temperature phase diagram of the Hubbard model (Figure 1).

A key computational challenge in the latter is evaluating the exponential of the Hamiltonian. For finite temperatures, this requires computing the density operator:

$$\rho(\beta) = e^{-\beta H}$$
 
Since this is exponentially hard in the system size, approximations are necessary. The traditional approach relies on the Suzuki-Trotter decomposition, but a more recent and accurate alternative is to use cluster expansions (see Figure 1) [3,4]. For both of these methods, the key challenge is to systemetically find accurate representations of this thermal state at high values of $$ \beta $$ (low temperatures). 

<p><img alt="Fig. 2: Example of cluster expansions" src="/images/thesistopics/2026/SDeMeyer4.png" style="float:right; width:280px" /></p>

#### Goal

This thesis will explore different methods for probing the finite-temperature phase diagram of the Hubbard model. There are multiple directions that could be taken depending on the interests of the student. One possibility is using the existing methodologies to study various parameter regimes of the Hubbard model, looking both at the feasibility and computational cost of obtaining accurate results. Another is working further on the development of these algorithms to further optimize their efficiency and accuracy. In both approaches, the first step will consist of looking at the strong-coupling limit of the Hubbard model, where the system can be modeled by the computationally less challenging tJ-model. Once the results of this model (which are interesting in their own right) are benchmarked, several different aspects of the Hubbard model can be investigated.

[1] Qin M. (2021) [arxiv:2104.00064](https://arxiv.org/abs/2104.00064)

[2] Sinha A. (2022) [arxiv:2209.00985](https://arxiv.org/pdf/2209.00985)

[3] Vanhecke B. (2021) [arxiv:2112.01507](https://arxiv.org/abs/2112.01507)

[4] Vanhecke B. (2019) [arxiv:1912.10512](https://arxiv.org/abs/1912.10512)

[5] Czarnik P. (2018) [arxiv:1811.05497](https://arxiv.org/abs/1811.05497)
