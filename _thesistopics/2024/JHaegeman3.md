---
title: "Shear viscosity and spectral functions of interacting quantum systems"
promoter: Jutho Haegeman, Michal Heller
supervisor: Daan Maertens
contact: Jutho Haegeman
topic: "Computational Quantum Many-Body Physics"
year: "2024"
---

#### Context

When studying quantum matter or quantum field theories, one of the interesting quantities is dynamical correlation functions. Upon Fourier transformation to the momentum and frequency/energy domain, these are known under various names such as spectral functions, Green's functions, or dynamic structure factors. These quantities are of great interest because they enable to relate analytical or computational predictions with experimental data. Indeed, dynamic structure factors of the magnetic moments in materials are directly accessible via for example inelastic neutron scattering experiments. Similarly, the retarded Green's function of the stress-energy tensor can be related to the shear viscosity via the Kubo formula, and is of great interest in the study of quantum field theories. Indeed, this parameter serves as an input to a relativistic hydrodynamical description of nonequilibrium processes in quantum field theories, e.g. to model the quark gluon plasma that is created in heavy ion collision experiments.

All of these quantities give direct information about the spectrum or dynamics of the quantum many body system. The study of strongly interacting quantum many body systems is of course notoriously hard, because of the exponential increase of the Hilbert space. Equilibrium properties can sometimes be captured by a quantum-to-classical mapping, in which thermal quantum states are represented as classical probability distributions, which are then probed via Monte Carlo sampling. However, this approach has a number of restriction. Many interesting quantum systems (especially those involving nonzero fermion densities, such as appearing in the quark gluon plasma) give rise to nonpositive "probabilities" under this mapping, which is known as the sign problem. Furthermore, Monte Carlo sampling techniques cannot access real-time phenomena. Instead, they attempt to evaluate dynamic correlation functions in imaginary time, and then to reconstruct the proper quantities at real time via "analytic continuation", a technique which is numerically unstable and not under good control.

An alternative technique is that of tensor networks, in which quantum wave functions are directly targeted and approximated as a contraction of a network of tensors. The feasibility of this approach is motivated by insights regarding the entanglement structure of low-energy quantum states. For one-dimensional quantum lattice systems, such as quantum spin chains, methods based on the variational class of one-dimensional tensor networks known as matrix product states, have become the de facto default computational approach and yield near-exact results. Tensor network methods are not restricted to equilibrium settings and can capture real-time evolution. While quantum entanglement does grow in nonequilibrium settings, which affects the computational cost, spectral properties at zero temperature can also be captured more directly via tensor network techniques that work directly in momentum and frequency space, at least at zero temperature. However, these techniques have not yet been developed to cope with finite temperature.

#### Goal

The goal of this thesis is to investigate different strategies to compute spectral functions of interacting quantum quantum lattice systems at finite temperature, using the formalism of matrix product states. As a first part, the student will follow the standard approach. Here, one first constructs the finite temperature quantum state, using the formalism of thermofield double states [1]. On top of these states, one can then compute the real-time dynamical correlation function using algorithms for time evolution, in particular, the time-dependent variational principle [2]. Green's functions are then obtained by numerically computing the Fourier transforms to frequency and momentum space. Various extensions are possible. For example, the maximal time interval that can be simulated will limit the resolution in frequency space, but can be extended by using complex (as opposed to purely real or purely imaginary) time [3], or by signal processing techniques [1]. As a second part to this thesis, a completely novel approach will be investigated. Here, one will directly linearize the equations that result from applying the time-dependent variational principle, which would then yield direct access to the spectral information in the form of a generalised eigenvalue problem. This technique has been investigated at zero temperature [4], but not at finite temperature, where one expect to see a more interesting spectrum of resonances with a finite lifetime.

An extensive set of MPS algorithms is available in the form of open source software packages within the Quantum Group of promotor Jutho Haegeman [5]. These algorithms can be used to perform the simulations of the first part, and on top of which the new algorithm for the second part can be constructed.

\[1\] Banuls, M. C., Heller, M. P., Jansen, K., Knaute, J., & Svensson, V. (2020). From spin chains to real-time thermal field theory using tensor networks. Physical Review Research, 2(3), 033301. (https://arxiv.org/abs/1912.08836)

\[2\] Haegeman, J., Cirac, J. I., Osborne, T. J., Pižorn, I., Verschelde, H., & Verstraete, F. (2011). Time-dependent variational principle for quantum lattices. Physical review letters, 107(7), 070601. (https://arxiv.org/abs/1103.0936)

\[3\]  Grundner, M., Westhoff, P., Kugler, F. B., Parcollet, O., & Schollwöck, U. (2023). Complex Time Evolution in Tensor Networks. arXiv preprint arXiv:2312.11705. (https://arxiv.org/abs/2312.11705)

\[4\] Hackl, L., Guaita, T., Shi, T., Haegeman, J., Demler, E., & Cirac, I. (2020). Geometry of variational methods: dynamics of closed quantum systems. SciPost Physics, 9(4), 048. (https://arxiv.org/abs/2004.01015)

\[5\] https://quantumghent.github.io/software/ or https://github.com/quantumghent/

