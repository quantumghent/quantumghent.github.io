---
title: "Crystal symmetries in tensor networks: simulating the Hubbard model on the triangular lattice"
promoter: Jutho Haegeman, Veronique Van Speybroeck
supervisor: Gleb Fedorovich, Nick Bultinck
contact: Jutho Haegeman
topic: "Correlated Quantum Materials"
year: "2024"
---

#### Context

In condensed-matter physics, the everlasting search for strongly-correlated materials that do not form simple metal or insulating phases has recently led to the discovery of twisted bilayer graphene. This material is obtained by taking two sheets of graphene, and placing them on top of each other with a small twisting angle. The twisting of the two honeycomb lattices leads to a so-called moiré superlattice, which at special “magic” angles exhibits a plethora of exciting strongly-correlated phases such as superconductivity or fractional Chern insulators. This groundbreaking discovery has opened up a completely new field of designing and exploring new materials with many new physical phenomena.

One particularly interesting set of materials is the class of transition metal dichalcogenides (TMD) such as the WSe2 or WS2 Moiré superlattices. For these materials, it was shown by theory [1] and experiment [2] that the flat bands around the Fermi level can realize the physics of strongly-correlated Hubbard models on the triangular lattice. The latter model is known to host metal-insulator transitions and putative spin-liquid regimes, but the precise determination of the phase diagram and the right parameters for observing these phases are currently not known.

The reason is that ab-initio calculations for these types of materials are notoriously difficult, because they exhibit very strong electron correlations. Indeed, standard ab-initio methods such as density-functional theory (DFT) fail in the presence of strong correlations and more accurate methods become unwieldy very quickly for realistic materials. Recently, the group of Profs. Frank Verstraete and Jutho Haegeman on the one side and the group of Prof. Veronique Van Speybroeck have teamed up for tackling precisely this question. The strategy is to use advanced ab-initio methods such as extensions of DFT, GW-methods and random-phase approximations to derive effective models for the electron bands that exhibit strong correlations, and afterwards use variational entanglement-based methods (known as tensor-network methods) for solving this effective model in the regime of strong electron correlations.


#### Goal

In this project, we will focus solely on the second step. This means that we will assume we have derived an effective model for the WSe2 or WS2 bilayer systems, which takes the form of a Hubbard model on the triangular lattice. We will therefore solve this model using tensor networks.

In the literature, there is a well-established tensor-network method for simulating these types of model, which boils down to placing the triangular-lattice model on a cylindrical geometry and using matrix product state (MPS) techniques for solving this effective one-dimensional model. Although quite successful [2-3], this method scales exponentially with the cylinder circumference, and it is unclear whether the physics of TMD materials is accurately represented by this method.

Therefore, we will develop a methodology where we tackle the model directly on the infinite triangular lattice and impose all possible lattice symmetries. This can be done using the formalism of projected entangled-pair states (PEPS), where variational wavefunctions can be built without breaking any symmetries. However, the application of PEPS methods in this context requires some methodological advances. In particular, we will need a method for computing observables of triangular-lattice PEPS wavefunctions.

In the course of this proposal, we hope that the student will develop a performant code for simulating PEPS wavefunctions on the triangular lattice. If this first part is successful, the student can proceed to simulate the physics of the triangular-lattice Hubbard model, which is still under heavy debate in the community. Furthermore, the methodology as developed by the student will serve as an integral part of the global strategy for the ab-initio simulation of triangular-lattice materials such as the TMD class of systems.

\[1\] Wu, F.; Lovorn, T.; Tutuc, E.; MacDonald, A. H., Hubbard Model Physics in Transition Metal Dichalcogenide Moiré Bands. Physical Review Letters 2018, 121 (2), 026402.

\[2\] Wang, L.; Shih, E.-M.; Ghiotto, A.; Xian, L.; Rhodes, D. A.; Tan, C.; Claassen, M.; Kennes, D. M.; Bai, Y.; Kim, B.; Watanabe, K.; Taniguchi, T.; Zhu, X.; Hone, J.; Rubio, A.; Pasupathy, A. N.; Dean, C. R., Correlated electronic phases in twisted bilayer transition metal dichalcogenides. Nat. Mater. 2020, 19 (8), 861-866.

\[3\] Wilhelm Kadow, Laurens Vanderstraeten, and Michael Knap, Hole spectral function of a chiral spin liquid in the triangular lattice Hubbard model, Phys. Rev. B 106, 094417 (2022)
