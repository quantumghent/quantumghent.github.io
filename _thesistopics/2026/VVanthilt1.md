---
title: "Belief in the Infinite: Tackling Infinite Tensor Networks with Belief Propagation."
promoter: Jutho Haegeman
supervisor: Victor Vanthilt, Adwait Naravane
contact: Victor Vanthilt
topic: Computational Quantum Many-Body Physics
year: "2026"
---

#### Context
Many interesting problems in and around physics can be formulated as the contraction of an infinite two-dimensional tensor network [1].

- Partition function of 2d classical models and (1+1)D quantum systems.
- Ground state entropy of 1d quantum mechanical systems.
- 2- (or more) point correlation functions.
- Counting problems like the perfect matching problem / dimer covering problem.

However, contracting an infinite tensor network exactly would require infinite computational resources. To address this, researchers have developed various approximate contraction techniques that achieve surprisingly high accuracy.

One common approach uses the ideas of the renormalization group to perform coarse-graining on tensors within a network. These techniques - Tensor Network Renormalisation (TNR) techniques - are well-established and serve as a useful benchmark for this thesis.

A promising alternative approach to contract 2d tensor networks, that borrows from statistical physics, is belief propagation (BP) [2]. It has been shown that BP is equivalent with a mean-field approximation to the problem.
To increase its accuracy, researchers have put forward several improvements. Loop series expansions and  loop cluster expansions to name a few [3, 4].

These novel methods remain an active field of research with many open questions to be answered and possible improvements to discovered.

#### Goal
This thesis will have a major numerical component, requiring programming in the Julia programming language (no prior knowledge required). It consists of three main objectives:

1. **Implement belief propagation**
Implement belief propagation for the contraction of infinite 2D tensor networks and validate it against exact analytical results. We will make use of the TensorKit Julia library which makes writing tensor network code a breeze.

2. **Systematic Benchmarking Against TNR Methods**
Perform a systematic comparison of BP-based contraction against established techniques (e.g. TRG, HOTRG) in terms of accuracy, computational cost, and scaling with bond dimension. Identify regimes where BP is competitive, and where it breaks down.

3. **BP Improvements**
Implement several improvements on top of BP put forward by [3] and [4].

4. **Exploration**
Explore novel improvements for BP and/or come up with hybrid TNR/BP methods.


[1] Bridgeman, J. (2016) [arxiv.org:1603.03039](https://arxiv.org/abs/1603.03039)
[2] Alkabetz R. [arXiv:2008.04433](https://arxiv.org/abs/2008.04433)
[3] Evenbly, G. (2024) [arxiv.org:2409.03108](https://arxiv.org/abs/2409.03108)  
[4] Gray J. (2025) [arXiv:2510.05647](https://arxiv.org/abs/2510.05647)

