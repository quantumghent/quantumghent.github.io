---
title: "The mystery of high-temperature superconductivity: ab-initio calculations using density-functional theory, downfolding and tensor networks"
promoter: Frank Verstraete, Veronique Van Speybroeck
supervisor: Nick Bultinck, Jutho Haegeman
contact: Jutho Haegeman
topic: "Correlated Quantum Materials"
year: "2024"
---

#### Context

The theoretical understanding and numerical simulation of strongly-correlated quantum materials has been one of the long-standing challenges in physics: Whereas the microscopic quantum-mechanical equations for describing e.g. electrons in a material have been known for over a century, solving these equations for a large number of them is prohibitively expensive. As a result, the use of approximate methods such as mean-field theory, Hartree-Fock theory, perturbation theory, etc have flourished and can actually yield very accurate descriptions of the relevant physics of many materials. For example, band theory often describes the electronic structure of many metallic or insulating systems, and Fermi-liquid theory describes the occurrence of quasiparticles in these systems. Another example is density functional theory (DFT), which is an independent particle model for many-electron systems that revolves around the use of exchange-correlation functionals for capturing the electron correlations; in the last fifty years, DFT has worked itself up to the default method for simulating large many-electron systems.

There are, however, still a number of materials that resist such approximate descriptions, and for which still no satisfactory understanding has been acquired. The most outstanding example in the field of condensed-matter physics is the mystery of high-Tc superconductivity: layered materials for which superconductivity persists up to temperatures at which any conventional description of superconductivity (i.e., BCS theory) would predict that a normal conductor has formed. It appears that strong quantum correlations in these systems are responsible for the superconducting properties, which falls outside the scope of traditional approximate methods such as mean field of perturbation theory. The most famous class of high-Tc superconductors are cuprates.

In the last years, a new theoretical and numerical framework has been developed that can account for strong quantum correlations or entanglement in quantum many-body systems: tensor networks. Because of their direct modeling of the quantum entanglement in many-body systems, they are typically applied to microscopic Hamiltonians for simplified toy models, which somehow capture the essential physics of a given materials. In the case of the cuprate superconductors, an effective model is the single-band Hubbard Hamiltonian, for which, indeed, tensor networks can predict the phase diagram with unprecedented precision.

#### Goal

In order to make progress in understanding real-life high-Tc materials such as the cuprates – and for designing other materials with superconducting properties, with an eye on technological applications – we need to go beyond toy models and come up with ab-initio calculations of these materials. In this thesis proposal, we will make use of a hybrid DFT/tensor-network method for simulating a specific cuprate material La2-xSrxCuO4, which has been verified experimentally and that probably goes beyond the simple Hubbard model.

The crucial idea in this proposal is to use DFT for obtaining an effective band model for this material, such that we can isolate the electronic degrees of freedom that exhibit strong correlations. Indeed, it is expected that most electron bands are, in fact, only weakly-correlated, and that only a few bands contribute to the phenomenon of superconductivity. The DFT solution allows to project out all these weakly-correlated bands, after which we can find real-space localized Wannier orbitals that describe the relevant electrons. We can compute hopping amplitudes between the orbitals and interaction terms. In the next stage, we use tensor networks to treat this effective strongly-correlated model head-on, using tensor networks. We will not only study the ground-state properties of this materials, but also the dynamics of the charge carriers (which are supposed to determine the mysterious Cooper pairs and the superconductivity), which can be readily measured in angle-resolved photo-emission spectroscopy.

We expect the student to collaborate with researchers of the Center for Molecular Modeling and the Quantum Group; the former group has a large expertise in DFT calculations and Wannier-localization, whereas the latter has developed the main tensor-network algorithms that will be used in this work.

\[1\] M. Imada, Charge Order and Superconductivity as Competing Brothers in Cuprate High-Tc Superconductors. J. Phys. Soc. Jpn. 2021, 90 (11), 111009.

\[2\] J. I. Cirac, D. Pérez-García, N. Schuch, and F. Verstraete, Matrix product states and projected entangled pair states: Concepts, symmetries, theorems, Rev. Mod. Phys. 93, 045003 (2021)

\[3\] Boris Ponsioen, Sangwoo S. Chung, and Philippe Corboz, Period 4 stripe in the extended two-dimensional Hubbard model, Phys. Rev. B 100, 195141 (2021)


