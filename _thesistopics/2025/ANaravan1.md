---
title: "Renormalising fermions and gauge fields using tensors"
promoter: Jutho Haegeman
supervisor: Adwait Naravane
contact: Jutho Haegeman
topic: "Computational Quantum Many-Body Physics"
year: "2025"
---

#### Context

The renormalisation group (RG) is one of the cornerstones of modern theoretical physics and exists in various implementations across different areas of classical as well as quantum physics. One particularly insightful RG scheme in the context of classical spin models in statistical mechanics is Kadanoff's spin blocking \[1\], a particular example of a real-space coarse-graining scheme \[2\].  While very instructive, this particular scheme does not result in a quantitatively precise description of critical phenomena. More recently, highly accurate real-space coarse-graining schemes have been constructed using the formalism of tensor networks. Hereto, the partition function of a statistical or quantum mechanical system is represented as a network of contracted tensors, where the contractions between different tensor indices encode the summations over the configuration space variables. By decomposing these tensors and contracting them, real-space transformations are obtained that result in coarse grained partition functions in terms of novel statistical variables. After the initial proposal by Levin and Nave \[3\], different improved and more advanced schemes have been proposed \[4,5,6\] (one of which is depicted below), and various strategies have been developed to extract the scaling behaviour of the system from these numerical simulations \[7,8\].

This technique can also be applied to quantum systems with fermionic degrees of freedom, which are then encoded using Grassmann numbers \[9\]. In the last one year, this approach has been reproduced using the formalism of fermionic super vector spaces\[10\] in the context of tensor based RG. Moreover, tensor based RG methods have been used to study Lattice gauge theories (LGTs) which normally cannot be studied using conventional methods. Thus tensor networks are a promising approach in the long term goal of simulating Lattice QCD. Many open questions remain:

<!-- * A more recent formalism to deal with fermions in tensor networks is based on super vector spaces \[10\], but this formalism has not yet been employed in the context of tensor-based RG. It would be interesting to understand whether this formalism provides a greater flexibility in how to implement the sequential coarse graining transformations. -->

* For quantum field theories on a lattice there are different ways to encode the partition function as a tensor network. Extending this formalism to Hamiltonians or actions with both fermionic and dynamical gauge degrees of freedom in (1+1) and (2+1) dimensions is of particular interest as ultimately QCD has both fermions and gauge bosons. How to encode continuous gauge degrees of freedom using symmetric tensors and efficiently represent and then contract the tensor network for the partition function remains an open question. 

* There are different numerical tensor renormalisation schemes that can be used to study these theories from the simplest one proposed by Levin and Nave to more complicated state-of-the-art ones such as Loop-TNR which can capture the RG flow in much better detail. Implementing these algorithms for fermionic and gauge degrees of freedom is of particular interest. 

* Finally, calculating observable quantities such as local observables, Wilson Loops and their expectation values with tensor networks is of great interest as these objects are important for studying the different phases of a lattice field theory. 

<div align="center">
![A specific tensor-based RG implementation](/images/thesistopics/2023/JHaegeman1.png)
</div>

#### Goal

The goals of these thesis is to address the points raised above and can depend on the interest of the student. We will start with replicating some of the existing results from fermionic tensor-based RG (TRG) studies, thereby translating the Grassmann number formalism to super vector spaces. We have developed an open-source Julia software package to perform Tensor Network Renormalisation (TNR) simulations called TNRKit.jl. A part of this project can also be to further develop this software library by adding novel TNR schemes. Next, we will look at the different strategies to discretise the fermionic and gauge degres of freedom to efficiently represent the lattice partition function as a tensor network and study different LGTs using the available TNR schemes. Finally, if time permits, we will implement and investigate algorithms to measure observables and study the critical spectra of different models. 

\[1\] Kadanoff, L. P. (1966). Scaling laws for Ising models near T c. Physics Physique Fizika, 2(6), 263.

\[2\] Efrati, E., Wang, Z., Kolan, A., & Kadanoff, L. P. (2014). Real-space renormalization in statistical mechanics. Reviews of Modern Physics, 86(2), 647. [arXiv:1301.6323](http://arxiv.org/abs/arXiv:1301.6323).

\[3\] Levin, M., & Nave, C. P. (2007). Tensor renormalization group approach to two-dimensional classical lattice models. Physical review letters, 99(12), 120601. [arXiv:cond-mat/0611687](http://arxiv.org/abs/cond-mat/0611687).

\[4\] Xie, Z. Y., Chen, J., Qin, M. P., Zhu, J. W., Yang, L. P., & Xiang, T. (2012). Coarse-graining renormalization by higher-order singular value decomposition. Physical Review B, 86(4), 045139. [arXiv:1201.1144](http://arxiv.org/abs/arXiv:1201.1144).

\[5\] Evenbly, G., & Vidal, G. (2015). Tensor network renormalization. Physical review letters, 115(18), 180405. [arXiv:1412.0732](http://arxiv.org/abs/arXiv:1412.0732).

\[6\] Hauru, M., Delcamp, C., & Mizera, S. (2018). Renormalization of tensor networks using graph-independent local truncations. Physical Review B, 97(4), 045111. [arXiv:1709.07460](http://arxiv.org/abs/arXiv:1709.07460).

\[7\] Gu, Z. C., & Wen, X. G. (2009). Tensor-entanglement-filtering renormalization approach and symmetry-protected topological order. Physical Review B, 80(15), 155131. [arXiv:0903.1069](http://arxiv.org/abs/arXiv:0903.1069).

\[8\] Ueda, A., & Oshikawa, M. (2023). Finite-size and finite bond dimension effects of tensor network renormalization. arXiv preprint [arXiv:2302.06632](http://arxiv.org/abs/arXiv:2302.06632).

\[9\] Gu, Z. C., Verstraete, F., & Wen, X. G. (2010). Grassmann tensor network states and its renormalization for strongly correlated fermionic and bosonic states. arXiv preprint [arXiv:1004.2563](http://arxiv.org/abs/arXiv:1004.2563).

\[10\] Bultinck, N., Williamson, D. J., Haegeman, J., & Verstraete, F. (2017). Fermionic matrix product states and one-dimensional topological phases. Physical Review B, 95(7), 075108. [arXiv:1610.07849](http://arxiv.org/abs/arXiv:1610.07849).
