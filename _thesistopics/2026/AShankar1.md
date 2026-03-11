---
title: "Sync or Swim? Phase-locking in 1D coupled Bose gases"
promoter: Jutho Haegeman, Karel Van Acoleyen
supervisor: Akshay Shankar
contact: Akshay Shankar
topic: "Condensed Matter Physics"
year: "2026"
---

#### Context

The phase of a quantum wave function is usually a microscopic detail, yet in coherent systems, it can drive macroscopic behavior. The Josephson effect is perhaps the most famous example of this phenomenon, where a phase difference between two coupled fluids results in a measurable supercurrent. While typically associated with solid-state materials, the effect is a general feature of coupled quantum matter. In the context of ultracold atomic gases, this can be realized by coupling two internal hyperfine states of a Bose gas with an externally driven Rabi field. This coupling acts to synchronize the relative phase between the species, a process which reduces to pendulum-like dynamics in the mean-field limit [1].

In one dimension, however, phase coherence is suppressed by strong quantum fluctuations that prevent the formation of a macroscopic condensate. The system instead behaves as a Tomonaga-Luttinger liquid [2], where phase correlations decay algebraically. The low-energy physics of such a system is captured by an effective Sine-Gordon field theory [3] in the presence of weak Rabi coupling. This framework shows that while even an infinitesimal coupling pins the relative phase and opens an excitation gap, the quantum fluctuations strongly oppose this pinning. This leads to a renormalized scaling of the gap that deviates significantly from the prediction of mean-field theory.

Capturing this behavior goes beyond the reach of standard descriptions like the Gross-Pitaevskii Equation (GPE) [4], which treats the system as a classical object and ignores the non-trivial effects of many-body correlations. As an alternative, one may utilize the recently developed multi-component continuous Matrix Product State (cMPS) formalism [5] to resolve these effects. This approach is particularly powerful because the ansatz is parametrized by the bond dimension D, which acts as a direct probe of entanglement. This allows for a systematic study of how many-body correlations modify the Josephson physics as the system moves beyond the D=1 mean-field limit.

References: 

[1] [S. Raghavan et al., Phys. Rev. A 59, 620 (1999)](https://arxiv.org/abs/cond-mat/9706220)

[2] [M. A. Cazalilla, J. Phys. B 37, S1 (2004)](https://arxiv.org/abs/cond-mat/0307033)

[3] Thierry Giamarchi. Quantum Physics in One Dimension, volume 121. Clarendon Press, Oxford, 2003.

[4] Lev Pitaevskii and Sandro Stringari. Bose-Einstein condensation and superfluidity, volume 164. Oxford University Press, 2016.

[5] [W. Tang, B. Tuybens, and J. Haegeman, arXiv:2512.24998 (2025)](https://arxiv.org/abs/2512.24998)

#### Goal

The goal of this project is to use the cMPS variational framework to characterize the ground-state properties of a Rabi-coupled 1D Bose gas and quantify the departure from mean-field theory directly in the continuum and the thermodynamic limit.

The project will begin with a literature study on one-dimensional quantum fluids. The student will familiarize themselves with the Lieb-Liniger model, Luttinger liquid theory, and the effective Sine-Gordon description of coupled systems. In parallel, the student will become acquainted with the theoretical construction and numerical implementation of the cMPS variational ansatz.

Building on this, the student will use the cMPS toolbox to investigate how quantum fluctuations renormalize the Josephson excitation gap. The focus will be on testing Sine-Gordon predictions through a finite entanglement scaling analysis in the weak coupling regime. This work will also involve quantifying the effect of inter-species interaction in the system.

This project is well suited for a student with a strong interest in theoretical and computatonal many-body physics. No prior knowledge of tensor networks or coupled bosonic systems is required.
