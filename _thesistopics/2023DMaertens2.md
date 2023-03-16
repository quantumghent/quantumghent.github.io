---
title: "Decay of the false vacuum"
promoter: Karel Van Acoleyen
supervisor: Daan Maertens
contact: Karel Van Acoleyen
topic: "Lattice Quantum Field theory"
year: "2023"
---

#### Context

False vacuum decay is the quantum mechanical process in which a meta stable state (called the
false vacuum) decays to the stable true vacuum. In a cosmological setting this decay could have
drastic consequences for local observers (i.e. we) such as changes in the fundamental forces and
the stability of matter and gravitational collapse. It is hypothesised that the electroweak in-
teraction is a meta-stable fundamental force where the electroweak vacuum instability depends
on the mass of the Higgs boson and the heaviest fermion.

In this master-thesis we want to study false vacuum decay in the context of the Gross-Neveu
model, a Quantum Field theory toy-model exhibiting many interesting properties such as di-
mensional transmutation and asymptotic freedom. Of particular interest is the fact that the GN
model exhibits dynamical mass generation which breaks the chiral symmetry apparent in the
Hamiltonian. Consequently the ground state is two-fold degenerate. When a (small) explicit
mass term is added to the theory this degeneracy is lifted with one of the two state obtaining
a slightly higher energy (the false vacuum). It is possible for the many-body wavefunction
to become trapped in the false vacuum and after some time decay to the true vacuum. This
process involves the formation of bubbles of true vacuum which nucleate until the whole space
is converted to the true ground state.

The class of Tensor Networks (TN) states are well-suited to perform numerical simulations
on this false vacuum decay. They allow for a fully quantum many body simulation thus giving
us access to the wavefunction of the entire universe. In addition, unlike Monte-Carlo methods,
TN states can be used to perform real-time evolution. In one spatial dimension such TN states
are called Matrix Product States (MPS) and there exist efficient algorithms to variationally
optimize this ansatz and do time evolution with them.

#### Goal

The goal of this thesis is to simulate quenches of the groundstate(s) of the GN model and
study the formation of kinks (domain-walls) and the related decay of a false vacuum to the true
vacuum. Up until now most of the literature concerns a semi-classical analysis of this process.
In thesis we want to perform a fully quantum many body simulation of the false vacuum decay
using real-time evolution with MPS. As such this thesis will pave the way towards the first ab
initio, fully quantum calculation of these false vacuum decays.

This thesis concerns both numerics and theory. The theoretical aspects include quantum many
body physics, Quantum Field theory and cosmology. On the numerical side, the programming
will be done the in the high performance programming language Julia using the already existing
open-source package MPSKit developed in this group.

In this master thesis the student will first do some literature study to become familiar with
false vacuum decay in Quantum Field theory and the matrix product states ansatz. After this
the student will be able to perform quenches with MPS, study its results and relate these to
the existing literature on false vacuum decay.
