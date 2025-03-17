---
title: "Best of both worlds: towards efficient computation of physical observables from integrable systems with Monte Carlo and Tensor networks."
promoter: Wei Tang, Jutho Haegeman
supervisor: Wei Tang, Xu Zhang, Gleb Fedorovich
contact: Wei Tang, wei.tang@ugent.be
topic: Computational Quantum Many-Body Physics
year: "2025"
---

#### Context
The Algebraic Bethe Ansatz (ABA) stands as one of the most significant exact methods in quantum integrable systems [1,2], providing analytical solutions to a wide class of many-body 
problems that would otherwise remain intractable. Despite its theoretical elegance and exactness, the ABA presents significant computational challenges when applied to the calculation 
of physical observables. Given these computational challenges, it is desirable to have an efficient numerical method to calculate the physical quantities of interest from Bethe ansatz 
wave functions. One promising direction is to exploit the matrix product state (MPS) representation of the Bethe ansatz wave function [3,4]. In Ref.[4], it was demonstrated that by 
applying standard matrix product state techniques, one can successfully truncate the bond dimension of the exact MPS to numerically manageable sizes while maintaining good accuracy 
for various observables. However, significant challenges emerge if this method is applied to larger systems, as the truncation process encounters substantial entanglement 
barriers that affect numerical accuracy.

#### Goal
This master thesis project aims to address these limitations by developing a novel computational approach that combines Monte Carlo sampling techniques with tensor network 
representations of Bethe ansatz wave functions. The proposed research includes **developing efficient Monte Carlo sampling algorithms tailored to the MPS representation of Bethe 
eigenstates**, implementing and benchmarking these methods for **computing correlation functions and other physical observables**, **comparing** the performance with traditional truncation 
approaches in terms of **accuracy and computational efficiency**. The student will gain a solid understanding of both the theoretical framework of algebraic Bethe ansatz and several 
numerical techniques, including tensor network algorithms and Monte Carlo sampling methods [5,6]. This knowledge will position the student for further research either on improving 
traditional tensor network algorithms or developing VMC+PEPS algorithms for challenging two-dimensional quantum systems.

#### References

[1] L. D. Faddeev, [arXiv:hep-th/9404013](https://arxiv.org/abs/hep-th/9404013)
[2] L. D. Faddeev, [arXiv:hep-th/9605187](https://arxiv.org/abs/hep-th/9605187)
[3] H. Katsura, I. Maruyama, [arXiv:0911.4215](https://arxiv.org/abs/0911.4215)
[4] V. Murg, V. E. Korepin, F. Verstraete, [arXiv:1201.5627](https://arxiv.org/abs/1201.5627)
[5] Ling Wang, Iztok Pizorn, Frank Verstraete, [arXiv:1010.5450](https://arxiv.org/abs/1010.5450)
[6] W.-Y. Liu, S. J. Du, R. Peng, J. Gray, G. K.-L. Chan, [arXiv: 2405.03797](https://arxiv.org/abs/2405.03797)
