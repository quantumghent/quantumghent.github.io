---
title: "Exploring topological phases in the Hubbard model using tensor networks and automatic differentiation"
promoter: Jutho Haegeman, Laurens Vanderstraeten
supervisor: Lukas Devos, Laurens Vanderstraeten
contact: Lukas Devos
topic: "Computational Quantum Many-Body Physics"
year: "2023"
---

In condensed-matter physics, tensor network algorithms have been proven to be an effective method for obtaining accurate numerical data in 1+1 dimensional quantum systems. However, when it comes to 2+1 dimensional systems, the complexity of the algorithms increases drastically. This poses a challenge for researchers who want to study these systems and obtain accurate numerical results.

To address this challenge, we propose to use automatic differentiation (AD), a technique inspired by the machine learning community, to determine derivatives for tensor networks automatically. This approach has the potential to simplify the current state-of-the-art methods and make them more efficient. We will apply this technique to study the Hubbard model, a paradigmatic model for describing strongly correlated electrons in condensed-matter physics.

The Hubbard model describes electrons hopping on a lattice with an energy penalty term when two electrons are on the same site. We will focus on the Hubbard model on the two-dimensional triangular lattice, which induces non-trivial frustration in the system. For strong interactions between the electrons, the ground state is an insulator where the spins of the electrons are arranged into a magnetically ordered phase. For weak interactions, the system behaves metallic. In between these two phases, a non-magnetic insulating state was recently discovered that breaks time-reversal symmetry and realizes a chiral topological phase. This kind of phase is theoretically well-described by the Laughlin wavefunction that pops up in the description of the fractional quantum Hall effect, and hosts anyonic excitations and gapless chiral edge modes.

While the existence of the chiral topological phase has been established using tensor-network methods on a restricted quasi two-dimensional geometry, a different study using variational Monte-Carlo disputed the existence of this phase, claiming that the chiral state was only found due to the restricted geometry. In this thesis, we aim to settle the debate around the phase diagram of the Hubbard model on the triangular lattice, using fully two-dimensional tensor networks.

To accomplish this goal, we will implement AD methods to optimize the relevant tensor networks, which can then be used to study general two-dimensional systems, including the triangular lattice Hubbard model. The results of this work have the potential to shed light on the behavior of strongly-correlated electron systems in two dimensions, and contribute to the ongoing efforts to develop more efficient and accurate methods for studying these systems.
