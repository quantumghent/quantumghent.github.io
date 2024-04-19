---
title: "Pseudo-spectral methods for interacting Bose-Einstein condensates"
promoter: Jutho Haegeman, Karel Van Acoleyen
supervisor: Akshay Shankar
contact: Akshay Shankar
topic: "Computational Quantum Many-Body Physics"
year: "2024"
---

#### Context

In recent years, cold atom experiments world-wide have rapidly claimed their position at the forefront of the remarkable advances taking place in our understanding of the quantum world. Such endeavours routinely push the boundaries of experimentally accessible regimes and uncover novel quantum phenomena, necessitating the advancement of ab-initio numerical techniques to understand these systems. Despite the popularity and effectiveness of tensor network techniques in simulating quantum systems, they have not seen many significant applications in these kinds of cold atom setups, aside from the setting of optical lattices.


In order to use tensor networks on such continuous systems, it is necessary to construct a network of local Hilbert spaces, effectively encoding the system on a lattice. However, a naive approach of discretizing the spatial dimension to generate a grid (i.e. finite differences) scales poorly with the number of grid points and introduces convergence issues during the variational optimization [1]. A common alternative involves expanding the wave-function with respect to a set of global basis functions (i.e. spectral methods) that are chosen based on the geometry and boundary conditions of the system. While these generally have excellent convergence properties, they introduce highly non-local terms in the Hamiltonian which invalidates the usual entanglement considerations that tensor network states are based upon.


A promising middle-ground seems to exist in the form of Discrete Variable Representations (DVR) [2], closely related to Pseudo-spectral methods. This approach amounts to the construction of a localized basis set through the application of an appropriate transformation on a spectral basis set. This allows the evaluation of local potentials on a discrete grid, while only introducing a slightly non-local kinetic energy term in the Hamiltonian. As a result, the DVR method is expected to maintain locality to a good extent as with grid-based methods, while also possessing similar convergence properties as spectral methods, giving us the best of both worlds. Such an approach has significant potential as it opens up the possibility of studying inhomogenous cold atom systems in the continuum.

 
\[1\] Michele Dolfi, Bela Bauer, Matthias Troyer, and Zoran Ristivojevic, Multigrid Algorithms for Tensor Network States, https://arxiv.org/abs/1203.6363

\[2\] John C. Light, Tucker Carrington Jr., Discrete Variable Representations and their Utilization, http://light-group.uchicago.edu/dvr-rev.pdf



#### Goal

The overall goal of this thesis is to understand the utility and limitations of Discrete Variable Representations in augmenting tensor network techniques (particularly, matrix product states) to study strongly interacting one-dimensional systems in the continuum. This will be largely facilitated by gaining familiarity with the numerical tensor network toolbox [3] developed by our group.


Over the course of the project, the student will develop modular numerical routines that facilitates experimentation with various DVRs to discretize the continuum, followed by the application of tensor network machinery to study the system. This will involve performing benchmarks with an alternative discretization scheme that has been explored recently [4], based on dividing the continuous space into segments and choosing carefully tuned basis functions within each of them (akin to finite element methods). Based on the results of these attempts, a motivated student may also wish to explore natural extensions to higher dimensions.


This project is well-suited for a student with a strong interest in computational physics and in the development of efficient numerical techniques.

\[3\] MPSKit.jl, https://quantumghent.github.io/software/

\[4\] Shovan Dutta, Anton Buyskikh, Andrew J. Daley, Erich J. Mueller, Density-Matrix Renormalization Group for Continuous Quantum Systems, https://arxiv.org/abs/2108.05366



