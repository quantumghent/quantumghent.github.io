---
title: "Illuminati&lpar;ng&rpar; the physics of strongly-correlated materials on the triangular lattice with quantum many-body simulations"
promoter: Jutho Haegeman, Veronique Van Speybroeck
supervisor: Sander De Meyer, Gleb Fedorovich, Daan Verraes
contact: Sander De Meyer 
topic: "Computational Quantum Many-Body Physics"
year: "2026"
---

#### Context

The search for new functional quantum phases is a central theme in condensed-matter physics, driven by the desire understand how strong electronic interactions and quantum mechanics conspire to produce unexpected collective behaviour. Among the most intriguing of these phases are quantum spin liquids: highly entangled states that evade conventional symmetry breaking even at zero temperature [1]. Unlike ordinary magnets, their electron spins remain in a fluctuating, liquid-like state, stabilised by strong quantum to fluctuations and geometric frustration. The triangular lattice provides a canonical setting for such physics: antiferromagnetic interactions on this geometry cannot all be satisfied simultaneously, giving rise to frustration, competing ground states, and a rich landscape of possible behaviours, including Mott insulating, metallic, and spin-liquid regimes. 

Since 1991, a prominent material candidate realising this landscape is κ-(BEDT-TTF)₂Cu₂(CN)₃, an organic charge-transfer salt whose low-energy electronic structure is well described by half-filled bands on an anisotropic triangular lattice of BEDT-TTF dimers (Fig. 1) [2]. At ambient pressure, it exhibits a Mott insulating state widely regarded as a quantum spin-liquid candidate. Upon applying pressure, the bandwidth increases relative to the on-site Coulomb repulsion, effectively tuning the ratio and driving the system across a metal-insulator transition, with superconductivity emerging at intermediate pressures. However, how pressure alters the effective interactions, and whether the corresponding simplified two-dimensional model accurately captures the resulting phases, remains unresolved, yet crucial for guiding the design of new functional materials. 

<p><img alt="Fig. 1: Crystal structure of κ-(BEDT-TTF)₂Cu₂(CN)₃ and its low-energy electronic behavior
captured by an effective anisotropic Hubbard model on the triangular lattice." src="/images/thesistopics/2026/SDeMeyer1.png" style="float:right; width:350px" /></p>

The reason is that ab initio simulations for these types of materials are notoriously difficult, because they exhibit very strong electron correlations. Indeed, typical methods such as density-functional theory (DFT) fail in the presence of strong correlations and more accurate methods become unwieldy very quickly for realistic materials. Recently, the group of Profs. Frank Verstraete and Jutho Haegeman on the one side and the group of Prof. Veronique Van Speybroeck have teamed up for tackling precisely this question. The strategy is to use advanced ab initio methods such as extensions of DFT, GW-methods and random-phase approximations to derive effective models for the electron bands that exhibit strong correlations, resulting in a (extended) Hubbard model describing these bands. Afterwards, variational entanglement-based methods (known as tensor-network methods) can be used to solve this effective model in the regime of strong electron correlations. 

#### Goal 

In this thesis, the goal is to get more insight into both the Hubbard model on the triangular lattice and the physics of strongly-correlated materials with a triangular geometry. This means that we will construct effective models for κ-(BEDT-TTF)₂Cu₂(CN)₃ at different hydrostatic pressures. The resulting triangular-lattice Hubbard model (Fig. 1) will be solved using tensor networks to probe the pressure-driven stability of the different phases. 

In the literature, there is a well-established tensor-network method for simulating these types of model, which boils down to placing the triangular-lattice model on a cylindrical geometry and using matrix product state (MPS) techniques for solving this effective one-dimensional model. Although quite successful, this method scales exponentially with the cylinder circumference, and it is unclear whether the physics is accurately represented by this method. 

In order to have a more systematic approach, the full two-dimensional model can be solved with tensor networks using the formalism of projected entangled-pair states (PEPS). While previous methods have done this by mapping the triangular to a square lattice, which breaks the lattice symmetry, we will develop a methodology where we tackle the model directly on the infinite triangular lattice [3]. 

During the course of the thesis, the student will develop a performant framework to simulate the physics of the triangular-lattice Hubbard model, which is still under heavy debate in the community. This involves both code to find the ground state of the Hubbard model and code to calculate its physical properties. If this first part is successful, the student can proceed to simulate the physics of the effective models for κ-(BEDT-TTF)₂Cu₂(CN)₃ at different hydrostatic pressures. Furthermore, the methodology as developed by the student will serve as an integral part of the global strategy for the ab initio simulation of triangular-lattice materials. 

<p><img alt="Fig. 2: Calculation of expectation values on a triangular lattice" src="/images/thesistopics/2026/SDeMeyer2.png" style="float:right; width:350px" /></p>

[1] Anderson, P. W. (1973). Resonating valence bonds: A new kind of insulator? Materials Research Bulletin, 8(2), 153–160. https://doi.org/10.1016/0025-5408(73)90167-0 

[2] Pustogow, A. (2022). Thirty-Year Anniversary of κ-(BEDT-TTF)2Cu2(CN)3: Reconciling the Spin Gap in a Spin-Liquid Candidate. Solids, 3(1), 93-110. https://doi.org/10.3390/solids3010007 

[3] Naumann, J., Eisert, J., & Schmoll, P. (2026). Variational optimization of projected entangled-pair states on the triangular lattice. Physical Review B, 113(4). https://doi.org/10.1103/g5gm-tzf8