---
title: "Hawking radiation for interacting theories"
promoter: Karel Van Acoleyen, Nick Bultinck
supervisor: Daan Maertens
contact: Karel Van Acoleyen
topic: "Lattice Quantum Field theory"
year: "2023"
---

#### Context

Ever since Hawking made his momentous discovery that black holes radiate, the famous Hawking effect, this has been one of the most intriguing and widely studied phenomenon in quantumfield theory (QFT) and high energy physics. 
Though the hawking effect is more or less understood, both in the continuum and on the lattice, for free theories it is unknown how much (if any) survives when interacting models are considered. 
As pointed out by Unruh in 1981 the equations of motion of the QFT theory are identical to that of sound waves propagating in a medium with a background velocity (i.e. a comoving liquid), called analogue gravity systems.
In such systems the horizon is formed when the flow velocity exceeds the local sound of speed forcing waves to travel in one direction only. 
These analogue gravity models allow us to study the Hawking effect both numerically and experimentally (unlike astronomical black holes).

In a recent paper we showed that a discretised version of such an analogue gravity model (i.e. a lattice model) also exhibits Hawking radiation. 
We are currently working on extending these results, which were done for a free model, to an interacting theory using Tensor Networks (TN) states. 
In particular TN states give us access to the full quantum many body wavefunction and unlike Monte Carlo methods also allow for real-time evolution. 
In one spatial dimension such TN states are called Matrix Product States (MPS) and there exist efficient algorithms to variationally optimize this ansatz and do time evolution with them.

#### Goal

The goal of this thesis is to contribute to the ongoing research in our group on Hawking radiation for interacting fermions on a one-dimensional lattice using the framework of matrix product states. 
In particular we are interested in real-time evolution of such models using MPS.
 
This thesis concerns both numerics and theory. The theoretical aspects include quantum many body physics, Quantum Field theory and General Relativity. 
On the numerical side, the programming will be done the in the high performance programming language Julia using thealready existing open-source package MPSKit developed in this group.

In this master thesis the student will first do some literature study to become familiar with the Hawking effect and matrix product states. 
After this the student will be able to contribute to our current research by doing simulations with MPS. 
The goal of this thesis is intentionally leftquite broad in recognition of the nature of ongoing research.
