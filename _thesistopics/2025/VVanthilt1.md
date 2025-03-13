---
title: Can You Belief It? Tackling Infinite Tensor Networks with Belief Propagation.
promoter: Jutho Haegeman
supervisor: Victor Vanthilt
contact: Victor Vanthilt
topic: Computational Quantum Many-Body Physics
year: "2025"
---

#### Context
Many physically relevant objects can be expressed as infinite tensor networks. Notable examples include partition functions of 2D classical statistical mechanics models and (1+1)D quantum models. Another important case is the expectation values of Projected Entangled Pair States (PEPS), which describe 2D quantum lattice systems.

However, contracting an infinite tensor network exactly would require infinite computational resources. To address this, researchers have developed various approximate contraction techniques that achieve surprisingly high accuracy. One common approach uses the ideas of the renormalization group to perform coarse-graining on tensors within a network. These techniques are well-established and serve as a useful benchmark for this thesis.

Recently, a promising new approach has emerged, combining belief propagation with loop series expansions to approximate tensor network contractions [2, 3].

- **Belief propagation** is a method for optimizing tensor networks by fixing latent degrees of freedom—referred to as the gauge—inherent to these networks.
- **Loop series expansions** build upon belief propagation by expressing the tensor network contraction as a series expansion, making otherwise intractable contractions feasible [4].

<p><img alt="Loop series expansion on a square tensor network" src="/images/thesistopics/2025/VVanthilt1.png" style="float:right; width:350px" /></p>

#### Goal

This thesis will take a numerical approach, requiring implementation in the Julia programming language. It consists of three main objectives:

1. **Implement belief propagation** for square tensor networks using the TensorKit package, a Julia library developed by the quantum group that provides essential tools for tensor network calculations.
2. **Utilize loop series expansions** to contract infinite square tensor networks.
3. **Benchmark the method** against existing contraction techniques, evaluating both numerical accuracy and computational efficiency.

The student will have the freedom to explore alternative approaches for loop series expansions and is encouraged to develop novel algorithms through creative experimentation.

#### References

[1] Bridgeman, J. (2016) [arxiv.org:1603.03039](https://arxiv.org/abs/1603.03039)  
[2] Tindall, J. (2023) [arxiv.org:2306.17837](https://arxiv.org/abs/2306.17837)  
[3] Evenbly, G. (2024) [arxiv.org:2409.03108](https://arxiv.org/abs/2409.03108)  
[4] Tindall, J. (2024) [arxiv.org:2306.14887](https://arxiv.org/pdf/2306.14887)
