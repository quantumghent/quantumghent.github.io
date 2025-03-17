---
title: "Projective Quantum Monte Carlo as a fermionic quantum circuit"
promoter: Jutho Haegeman, Nick Bultinck
supervisor: Xu Zhang
contact: Xu Zhang, xzhangzh.zhang@ugent.be
topic: Computational Quantum Many-Body Physics
year: "2025"
---

#### Context
In classical circuit, one can use a series of binary code (i.e., ‘0’ and ‘1’) to represent the information and use logic gate to realize all kinds of operations. While in quantum circuit, the binary code is replaced by the quantum state (i.e., ‘|0>’ and ‘|1>’ in Fock space) and the gate operation becomes local unitary evolution. From a product state, the system can generate long-range entanglement after a long enough unitary evolution, while the measurement (local Hermitian projection) could reduce it. Thus, one should expect there is a Measurement-Induced Phase Transitions (MIPT) [1-3]. However, most of the recent quantum circuit research focus on the bosonic states and operations (i.e., hard core bosons) and fermionic quantum circuit which shares the same Hilbert space seems less attractive. The reason can come from the redundancy of Jordan-Wigner string in a matrix product operator (MPO) which is the main tool used. If one is familiar with the Projective Quantum Monte Carlo (PQMC) [5], he/she should find out it is a perfect tool to study fermionic quantum circuit since there is an isomorphic mapping. The decoupled repulsive interaction corresponds to the unitary evolution, and the kinetic term becomes the Hermitian projection. The interesting observations in bosonic quantum circuit like MIPT should also be expected in a fermionic quantum circuit with a potentially different critical behavior.

#### Goal
The goal of this thesis is to explore the possibility of simulating a fermionic quantum circuit within PQMC framework. A first step could be comparing the one-dimensional critical behavior of MIPT between fermionic and bosonic random quantum circuit. Due to PQMC has no dimensional limitation from entanglement area law, one can also study the critical behavior in higher dimension (e.g., two-dimension) fermion quantum circuit.

#### References

[1] Fisher, M.P., Khemani, V., Nahum, A. and Vijay, S., [arXiv:2207.14280](https://arxiv.org/abs/2207.14280)
[2] Skinner B, Ruhman J, Nahum A., [arXiv:1808.05953](https://arxiv.org/abs/1808.05953)
[3] Li Y, Chen X, Fisher M.P., [arXiv:1808.06134](https://arxiv.org/abs/1808.06134)
[4] Li Y, Chen X, Fisher M.P., [arXiv:1901.08092](https://arxiv.org/abs/1901.08092)
[5] F Assaad, H Evertz, [Computational many-particle physics](https://scholar.google.com/scholar?cluster=9863927204596278835&hl=en&oi=scholarr)
