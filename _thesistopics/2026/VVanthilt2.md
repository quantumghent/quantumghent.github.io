---
title: "Learning Scattering Amplitudes through Tensor Networks"
promoter: Ben Page, Jutho Haegeman
supervisor: Simone Devoto, Victor Vanthilt
contact: Simone Devoto, Victor Vanthilt
topic: High Energy Physics
year: "2026"
---

#### Context

Experimental measurements at the Large Hadron Collider (LHC) are reaching unprecedented precision, a trend that will intensify during the High-Luminosity LHC upgrade. At the same time, the high collision energies of the LHC, together with the strength of the Quantum Chromodynamics (QCD) interaction, mean that proton-proton collisions produce many particles in the final state. Providing sufficiently precise theoretical predictions for cross-sections at the LHC is challenging because it requires evaluating scattering amplitudes -- sums of many, complicated Feynman diagrams -- whose complexity grows rapidly with the required precision and number of particles involved.

Modern methods compute scattering amplitudes numerically using sophisticated mathematical and computer-algebra techniques, but the resulting evaluations are often too slow to be used efficiently in large-scale cross-section calculations across phase space. In practice, however, the amplitudes do not need to be known to extremely high precision -- an accuracy at the level of roughly one part in ten thousand is typically sufficient for phenomenological applications. To meet experimental needs, an approach that has recently attracted attention [1] is to understand whether numerical evaluations of amplitudes can be used to construct approximations that accurately reproduce the amplitudes across phase space while avoiding the high computational cost of traditional techniques.

This problem can be seen as a machine learning challenge, where scattering amplitudes are learned and modelled across a high-dimensional phase space, using a relatively small number of samples.

#### Goal

In this project, we will investigate interpolation methods for constructing efficient approximations of scattering amplitudes across phase space. In particular, we will explore a recently developed technique, known as tensor cross interpolation [2], that enables the efficient construction of low-rank representations of high-dimensional functions. This “quantum-inspired” approach [3] is based on tensor networks, a framework that was originally developed to model ground states of quantum many-body systems, but that is increasingly being used for a variety of machine learning applications. In particular, tensor cross interpolation techniques exploit hidden structures in multivariate functions in order to learn accurate tensor network approximations that require far fewer function evaluations than traditional interpolation methods. The goal is to assess whether such methods can be used to learn fast surrogate models of scattering amplitudes from numerical data, reproducing the amplitudes across phase space with the accuracy required for phenomenological applications while significantly reducing computational cost. These techniques were recently applied successfully in the context of some typical problems in condensed matter physics [4,5], but in this thesis, the student will investigate these techniques and apply them to several state-of-the-art scattering amplitudes relevant for phenomenology at the Large Hadron Collider, thereby gaining experience in modern numerical techniques and scientific programming.

<p><img alt="Tensor Cross Interpolation" src="/images/thesistopics/2026/VVanthilt2.png" style="float:right; width:350px"/></p>

#### References

[1] Bresó-Pla, V. (2025) [arXiv:2412.09534](https://arxiv.org/abs/2412.09534v2)

[2] Núñez Fernández, Y. (2025) [arXiv:2407.02454](https://arxiv.org/abs/2407.02454)

[3] Waintal, X. (2026) [arXiv:2601.03035](https://arxiv.org/abs/2601.03035)

[4] Núñez Fernández, Y. (2022) [arXiv:2207.06135](https://arxiv.org/abs/2207.06135)

[5] Waintal, X. (2026). [arXiv:2602.03598](https://arxiv.org/abs/2602.03598)

