---
title: "Tensor renormalisation group for fermions"
promoter: Jutho Haegeman
supervisor: Gleb Federovich, Atsushi Ueda
contact: Jutho Haegeman
topic: "Computational Quantum Many-Body Physics"
year: "2024"
---

#### Context

The renormalisation group (RG) is one of the cornerstones of modern theoretical physics and exists in various implementations across different areas of classical as well as quantum physics. One particularly insightful RG scheme in the context of classical spin models in statistical mechanics is Kadanoff's spin blocking \[1\], a particular example of a real-space coarse-graining scheme \[2\].  While very instructive, this particular scheme does not result in a quantitatively precise description of critical phenomena. More recently, highly accurate real-space coarse-graining schemes have been constructed using the formalism of tensor networks. Hereto, the partition function of a statistical or quantum mechanical system is represented as a network of contracted tensors, where the contractions between different tensor indices encode the summations over the configuration space variables. By decomposing these tensors and contracting them, real-space transformations are obtained that result in coarse grained partition functions in terms of novel statistical variables. After the initial proposal by Levin and Nave \[3\], different improved and more advanced schemes have been proposed \[4,5,6\] (one of which is depicted below), and various strategies have been developed to extract the scaling behaviour of the system from these numerical simulations \[7,8\].

This technique can also be applied to quantum systems with fermionic degrees of freedom, which are then encoded using Grassmann numbers \[9\]. While this approach has been used in a number of studies, there are various interesting open questions:

* A more recent formalism to deal with fermions in tensor networks is based on super vector spaces \[10\], but this formalism has not yet been employed in the context of tensor-based RG. It would be interesting to understand whether this formalism provides a greater flexibility in how to implement the sequential coarse graining transformations.

* For relativistic quantum field theories, there are various ways to discretise the action or Hamiltonian, and thus to encode the partition function as a tensor network. This is particularly relevant in relation to the notion of the fermion doubling problem, i.e. the fact that discretising Dirac fermions necessarily gives rise to spurious low-energy degrees of freedom. These can be avoided in the one-dimensional Dirac Hamiltonian when discretising space, and it is an interesting question how this relates to the partition function where the action is isotropically discretised in (1+1) dimensional spacetime.

* Finally, different flavors of (1+1)-dimensional massless Dirac fermions can interact in a particular way that shares several features with quantum chromodynamics. This is known as the Gross-Neveu model. In particular, the Gross-Neveu interaction term is marginally relevant and results in dynamical mass generation. The behaviour of such marginally relevant interactions in tensor-based RG schemes is not well understood, and could be investigated further using the techniques from Ref \[7\].

<div align="center">
![A specific tensor-based RG implementation](/images/thesistopics/2023/JHaegeman1.png)
</div>

#### Goal

It is the goal of this thesis to address some (or all) of the above questions. We will start with replicating some of the existing results from fermionic tensor-based RG (TRG) studies, thereby translating the Grassmann number formalism to super vector spaces. Code to manipulate tensors in super vector spaces is available (in both Julia and Matlab) and can be used to implement the TRG schemes. Next, we will look at the different strategies to discretise the free Dirac fermion in (1+1) spacetime dimensions and build the tensor network representation of the partition function, and study it using our TRG approach, in order to understand the differences in relation to the fermion doubling problem. Finally, if time permits, we can also study the Gross-Neveu model, thereby the selecting the discretisation strategy that seems most appropriate for the problem, and try to understand how to extract the scaling behaviour (the running coupling constant or beta function).


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
