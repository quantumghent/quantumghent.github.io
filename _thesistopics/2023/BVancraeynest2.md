---
title: "Spatial symmetries in tensor networks"
promoter: Frank Verstraete
supervisor: Bram Vancraeynest
contact: Bram Vancraeynest-De Cuiper
topic: "Condensed Matter Theory"
year: "2023"
---

#### Context

One of the central research topics in the field of quantum many-body physics is the search for and characterization of so-called symmetry-protected topological (SPT) phases. The idea behind SPT phases is that the space of states that belong to the same phase in the absence of symmetries, falls apart in different disconnected components due to topological obstructions when symmetries are imposed. This picture can be made explicit in the language of tensor networks, which provide a way to represent many-body wave functions in terms of local tensors that lay bare the entanglement routing. In the celebrated work by Chen et al. [1] it was shown that such topological obstructions in 1+1D arise because symmetries can act projectively ie. up to a phase on the entanglement degrees of freedom of the tensor network under study. In their work, they considered on-site symmetries (such as spin rotations), parity and time-reversal. The relevant tensor networks in this case are the so-called matrix product states (MPS).

Recently, we showed in [2] using similar tensor network techniques that also spatial symmetries (such as glide reflections possibly combined with a rotation), classified by the 7 so-called frieze symmetry groups [3], can protect SPT phases. We identified the topological obstructions and found representative tensor network states for every of the found phases. An interesting and very relevant question is the generalization of these ideas to 2+1D. In this case the relevant tensor networks are the projected entangled pair states (PEPS).

#### Goal

The goal of this project is to gain a deeper understanding of the implementation of spatial symmetries in tensor networks. 
In a first stage the student should familiarize themself with tensor network methods and the relevant concepts of SPT phases. Next, a few different goals can be pursued, both theoretical and computational in nature. One possibility is to extend the work in [2] to also incorporate on-site symmetries that can interact non-trivially with the spatial symmetries. With the found MPS ansätze, one could carry out some interesting numerical simulations using the extensive numerical toolbox developed in our group [4]. Another ambitious goal is to consider the 17 wallpaper groups [5] and the SPT classification they give rise to. This SPT classification was recently obtained using field theory methods [6], but we wish to invoke these symmetries directly on the PEPS tensors. The student could also try to understand how spatial symmetries can be exploited in PEPS simulations in which spatial symmetries, possibly combined with global on-site symmetries, are very relevant for the simulation of materials. A model that could be investigated is for example the spin 1/2 antiferromagnetic Heisenberg model on the kagome lattice, which is believed to be a good description of Herbertsmithite.

[1] X. Chen, Z.-C. Gu, and X.-G. Wen, [arXiv:1103.3323](https://arxiv.org/abs/1103.3323)

[2] B. Vancraeynest-De Cuiper, J. C. Bridgeman, N. Dewolf, J. Haegeman, and F. Verstraete. [arXiv:2202.12880](https://arxiv.org/abs/2202.12880)

[3] [Frieze groups on Wikipedia](https://en.wikipedia.org/wiki/Frieze_group)

[4] [Software page](quantumghent.github.io/software/)

[5] [Wallpaper groups on Wikipedia](https://en.wikipedia.org/wiki/Wallpaper_group)

[6] R. Thorngren, D.V. Else, [arXiv:1612.00846](https://arxiv.org/abs/1612.00846)
