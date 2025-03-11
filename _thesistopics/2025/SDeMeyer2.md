---
title: "The mystery of high-temperature superconductivity: A Computational Approach from DFT to PEPS"
promoter: Jutho Haegeman, Veronique Van Speybroeck
supervisor: Sander De Meyer, Gleb Fedorovich, Daan Verraes
contact: Sander De Meyer
topic: "Computational Quantum Many-Body Physics"
year: "2025"
---

#### Context

Superconductors have vanishing electrical resistance under a certain temperature, called the critical temperature Tc. They were first discovered by the Dutch physicist Heike Kamerlingh Onnes in 1911, when he found that mercury exhibits superconductivity with Tc = 4.2K [1]. Thus began the search for materials exhibiting superconductivity at room temperature. A big step in this search was the discovery of high-temperature superconductivity in 1986 [2]. Here, they found a critical temperature of 30K, the highest at the time, for a system consisting of barium, lanthanum, copper, and oxide, specifically BaxLa5−xCu5O5(3−y) with x = 1 and 0.75 and y > 0. The original theory to describe superconductivity proposed by Bardeen, Cooper, and Schrieffer, called BCS theory, failed to describe this high-temperature superconductivity [3, 4]. A complete theory of this effect is still missing, more than 40 years after its discovery.

<p><img alt="Fig. 2: Phase diagram of the Hubbard model" src="/images/thesistopics/2025/SDeMeyer3.png" style="float:right; width:350px" /></p>

#### Goal

The goal is to start from a Density-Funtional Theory calculation of the material HgBa2CuO4 (Figure 1) and to capture the strongly correlated degrees of freedom with a downfolding procedure. This yields an effective Hamiltonian that can be solved using Tensor Networks [5,6]. The student can either perform a calculation of the Hubbard model or the t-J model based on the desired balance between accuracy and computational cost. The ground state wave function can then be found using the 2-dimensional version of tensor networks, called Projected Entangled-Pair States (PEPS). The student can look whether this ground state is superconducting or exhibits stripe-order to probe the zero-temperature phase diagram (Figure 2) [7]. The next step could be to not only incorporate interactions that act between nearest neighbours on the lattice, but also include further-reaching interactions. Another extension would be look at different doping levels, to probe the influence of the electron filling on the ground state properties.

<p><img alt="Fig. 2: Phase diagram of the Hubbard model" src="/images/thesistopics/2025/SDeMeyer2.png" style="float:right; width:350px" /></p>

[1] Dirk, v. & Kes, P. Europhysics News 63 (2011).

[2] Bednorz, J. G. & Muller, K. A. Z. Phys. B 64, 189–193 (1986).

[3] Bardeen, J. et al. Physical Review 106, 162–164 (1957).

[4] Bardeen, J. et al. Physical Review 108, 1175–1204 (1957).

[5] Bridgeman, J. (2016) [arxiv:1603.03039](https://arxiv.org/abs/1603.03039)

[6] Vrancken, D. (2025) [arxiv:2502.19588](https://arxiv.org/pdf/2502.19588)

[7] Ponsion, B. (2019) [PRB:100.195141](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.100.195141)
