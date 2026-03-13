---
title: "Fast and Furious about Entanglement - Simulating the dynamics of strongly-correlated quantum systems with tensor networks"
promoter: Jutho Haegeman
supervisor: Sander De Meyer
contact: Sander De Meyer 
topic: "Computational Quantum Many-Body Physics"
year: "2026"
---

#### Context

Solving strongly correlated quantum systems is notoriously difficult, but nevertheless very important to unravel the mysteries behind high-temperature superconductvitiy and strange quantum phases like spin liquids. One of the most widely-used models to describe the properties of stronlgy-correlated materials is the Hubbard model. It describes fermions hopping on a lattice, with a hopping term and a repulsive term [1]

$$H = -t \sum_{<i j> \sigma} \left(\hat{c}_{i \sigma}^\dagger \hat{c}_{j \sigma} + h.c.\right) + U \sum_i \hat{n}_i \hat{n}_j$$.

<p><img alt="Fig. 1: Phase diagram of the Hubbard model" src="/images/thesistopics/2026/SDeMeyer3.png" style="float:right; width:350px" /></p>

However, solving this model remains a significant challenge, leading to the development of numerous computational approaches. Among these, Tensor Networks (TN) have emerged as a powerful tool, explicitly capturing strong correlations without suffering from the sign problem (like Quantum Monte Carlo methods). In particular, the two-dimensional TN variant, Projected Entangled-Pair States (PEPS), is widely used but has been primarily applied to ground-state (0K) calculations and static properties. To get more insight into the Hubbard model, it is crucial to extend these methods to finite-temperature states and their time evolution [2]. While a lot of progress has been made in the former, the dynamics of these quantum states is much less investigated. Understanding what happens to a system when there is a sudden quench or when a perturbation on top of the ground state evolves through time nonetheless contains crucial information about the underlying properties of the system.

To investigate the real-time evolution of a quantum state, the evolution operator has to be calculated, which is given by

$$ O(\Delta t) = e^{-i \Delta t H}$$

Since this is exponentially hard in the system size, approximations are necessary. The traditional approach relies on the Suzuki-Trotter decomposition, but a more recent and accurate alternative is to use cluster expansions (see Figure 2) [3,4]. For both of these methods, the key challenge is to systemetically find accurate representations of this evolution operator at high values of $t$. The cluster expansion method has up until now mostly been used for thermal states in an imaginary-time evolution approach, whereas here real-time evolution would be needed [5].

<p><img alt="Fig. 2: Example of cluster expansions" src="/images/thesistopics/2026/SDeMeyer4.png" style="float:right; width:280px" /></p>


#### Goal 

The thesis will explore different methods for simulating real-time evolution of a quantum system. Since the state-of-the-art methods are scarce in (2+1)-dimensional systems, the first step will consist of benchmarking the current methods on a simpler model. Depending on the interests of the student, the next step can be to either apply the methods used for the simple model to the tJ and Hubbard model to investigate the properties of these models and the materials they describe, or focus more on the development and implementation of different schemes that could be more performant.

[1] Qin M. (2021) [arxiv:2104.00064](https://arxiv.org/abs/2104.00064)

[2] Sinha A. (2022) [arxiv:2209.00985](https://arxiv.org/pdf/2209.00985)

[3] Vanhecke B. (2021) [arxiv:2112.01507](https://arxiv.org/abs/2112.01507)

[4] Vanhecke B. (2019) [arxiv:1912.10512](https://arxiv.org/abs/1912.10512)

[5] De Meyer S. (2026) [arxiv:2602.22113](https://arxiv.org/abs/2602.22113)