---
title: "Efficient simulation of near-term quantum processors"
promoter: Frank Verstraete
supervisor: Lander Burgelman, Lukas Devos
contact: Lander Burgelman
topic: "Quantum Information"
year: "2023"
---

#### Context

The realization of quantum information processing devices has seen a surge of interest in recent years, with significant progress being made towards functional intermediate-scale quantum processors. While the search for a game-changing application of quantum computation is still very much ongoing, many successful experiments [1, 2] have been gradually ticking off the first boxes on the list of milestones that need to be reached along the road to practically useful quantum information processing devices [3].

An essential aspect to these short term experiments is the ability to accurately characterize and predict the properties of small devices being built in the lab. On the one hand this benchmarking is a crucial step in the design process to ensure devices will display the desired properties at cryogenic temperatures. On the other hand, the ability to predict the dynamical properties of a device and to compare this to the measured performance can help with detecting anomalies in experimental results.

While many tools for the exact simulation of open quantum systems under decoherence have been developed [4], these are limited to small system sizes and are becoming increasingly inadequate for realistic experimental devices. Approximate methods such as tensor networks states provide a promising alternative, as this variational class of wavefunctions can accurately capture the low-entanglement states that naturally arise in well-stabilized quantum devices.

#### Goal

The goal of this project is to adapt tensor network tools to the simulation of near-term quantum devices. As a first step, the student will need to become familiar with the experimental quantum hardware platforms currently being pursued and with the established techniques used to simulate the properties and performance of devices built on these platforms. They will then learn how to recast the static and dynamic Hamiltonians associated to a device with a specific layout [5] into a tensor network representation.

From there, both established and novel algorithms for diagonalization and time evolution in tensor networks with different geometries will be adapted to this setting, tailoring these techniques to the specific form of the Hamiltonians arising in this context. The performance and accuracy of different approaches will be compared to existing exact and approximate methods, identifying their strengths and weaknesses. The ideal outcome for this project would be a novel and performant framework that can be used by experimental groups as a tool in the design and benchmarking of near-term quantum processors.

[1] Sebastian Krinner et al. Realizing Repeated Quantum Error Correction in a Distance-Three Surface Code. [Nature 605, 669–674](https://arXiv.com/abs/2112.03708) (2022)

[2] Google Quantum AI. Suppressing quantum errors by scaling a surface code logical qubit. [Nature 614, 676–681](https://doi.org/10.1038/s41586-022-05434-1) (2023)

[3] Earl T. Campbell, Barbara M. Terhal, and Christophe Vuillot. Roads towards fault-tolerant universal quantum computation. [Nature 549, 172–179](https://arXiv.org/abs/1612.07330) (2017)

[4] [qutip](https://qutip.org/), [QuantumOptics.jl](https://docs.qojulia.org/)

[5] [scqubits](https://scqubits.readthedocs.io/en/latest/)
