---
title: "Exploiting symmetry and tensor networks to reveal the electronic structure of d2-d8 transition metal complexes"
promoter: Veronique Van Speybroeck, Jutho Haegeman
supervisor: Laurens Vanderstraeten
contact: Laurens Vanderstraeten
topic: "Correlated Quantum Materials"
year: "2023"
---

#### Context

A proper description of the electronic structure, in particular the splitting of the d-orbitals, in d2-d8 transition metal complexes is very challenging from the theoretical point of view, as these complexes are prone to strong electron correlation.  From the application point of view, a fundamental understanding of both the ground and excited state properties of these complexes is of utmost importance, as they are important building blocks in nanostructured materials such as metal-organic frameworks. 

Nowadays, the method of choice to solve many-body systems rely on the electron density. Density Functional Theory (DFT) describes the ground state and Time-Dependent Density Functional Theory provides a description of excitations between electronic levels. The ground state energy (and other observable quantities) are theoretically guaranteed to be completely determined as a functional of this density, so that DFT is –in principle– an exact solution method. Unfortunately, the exact form of the energy functional is unknown. The accuracy of DFT based methods thus relies on the choice of energy functional (more specifically the exchange-correlation functional).

For d2-d8 transition metal complexes containing transition metals such as V2+/3+, Cr2+/3+, Mn2+/3+, Fe2+/3+, Co2+/3+, Ni2+/3+ with partially filled d-orbitals, DFT completely fails in describing the electronic structure, both of ground and excited states, as the wavefunction cannot be described by a single Slater determinant.  To mitigate this problem, one can resort to high-level wavefunction based methods such as complete active space self-consistent field (CASSCF) and multireference configuration interaction (MRCI).  These methods have important drawbacks, firstly they are computationally very expensive but secondly the results are also very much dependent on the choice of the active space from which excited states are selected.

Another fundamentally different approach to treat the many-body system is based on tensor network states.  TNs have emerged over the past two decades as extremely versatile and powerful trial wave functions for interacting quantum lattice systems. They do not involve corrections on top of a non-interacting reference configuration, but take into account the spatial distribution of quantum correlations (as expressed by an area law scaling of quantum entanglement). Tensor network states are also very promising for isolated molecular systems. For Mn based complexes, a formalism based on tensor network states was successfully applied. However, Mn is one of the easier elements in the 3d transition metal series, as it has a non-degenerate ground state [1]. Other elements like Co are extremely difficult to describe correctly, as they have a degenerate ground state and they may exhibit both single and double excitations.  In the literature, alternative approaches have been proposed to treat correlation effects in these complexes such as ligand field Density Functional Theory. However, these techniques are still very approximative, rely on DFT, and do not provide intensities of the excitations.

Recently, a collaboration was set up between the Center for Molecular Modeling (Van Speybroeck) and the Quantum Group (Verstraete, Haegeman) to explore the feasibility of Tensor Network states for ab initio simulations of strongly correlated materials. Within this thesis, we aim to extend the tensor-network formalism to obtain with high accuracy the d-d excitations of the d2–d8 hexaaqua and lower coordinated TMCs [M(H2O)6]n+, with M a 3d transition metal ion (V2+/3+, Cr2+/3+, Mn2+/3+, Fe2+/3+, Co2+/3+, Ni2+/3+) and x={6,5,4}.  Earlier work performed at the CMM, has shown that the symmetry is a very important factor in the relative position of the various d-states (Figure 1).  Also for tensor networks symmetry is very important. 

#### Goal

In this project, we wish to extend this tensor-network formalism to the more challenging case of Co complexes. In the previous study on Mn [1], a “standard” tensor-network method (based on matrix product states) was used that breaks all the spatial symmetries of the system under study. Here we wish to develop a specially dedicated type of tensor network that mimics all the symmetries of the system, and which therefore we expect to perform better in capturing its essential features. The downside of this new type of tensor network is that we cannot use standard optimization routines, but that we will have to variationally optimize the tensor network wavefunction directly [2]. Alternatively, we could try to combine the standard matrix product state (MPS) format with a novel approach for optimizing over the mapping from orbitals to sites. In this scheme, the MPS tensors as well as global basis rotation for the orbitals are simultaneously optimized using a gradient-based algorithm. This is in sharp contrast with existing schemes, where the orbitals are only shuffled in a pairwise manner, and this optimization is performed separately from the MPS optimization using an alternating strategy.

Building on such a successful optimization routine, we can also target the excited states [3], which is of particular relevance for the applications mentioned above. 

#### References

[1] Sebastian Wouters, Thomas Bogaerts, Pascal Van Der Voort, Veronique Van Speybroeck, and Dimitri Van Neck, DMRG-SCF study of the singlet, triplet, and quintet states of oxo-Mn(Salen),  J. Chem. Phys. 140, 241103 (2014)

[2] Laurens Vanderstraeten, Jutho Haegeman, Philippe Corboz, and Frank Verstraete, Gradient methods for variational optimization of projected entangled-pair states, Phys. Rev. B 94, 155123 (2016)

[3] Laurens Vanderstraeten, Michaël Mariën, Frank Verstraete, and Jutho Haegeman, Excitations and the tangent space of projected entangled-pair states, Phys. Rev. B 92, 201111 (2015)
