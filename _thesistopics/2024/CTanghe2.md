---
title: "Engineering synthetic dimensions in cold atom systems"
promoter: Karel Van Acoleyen
supervisor: Akshay Shankar, Clara Tanghe
contact: Akshay Shankar
topic: "Bose-Einstein condensate as a quantum simulator"
year: "2024"
---

#### Context

The physics of interacting many-body systems has been of great interest to researchers for decades, as they host a variety of wildly exotic phenomena emerging from the rich interplay of quantum effects. However, a large class of these systems remain theoretically and numerically intractable due to an exponential growth of the system description. The concept of **quantum simulation** is a particularly elegant formulation designed to tackle this, originally proposed by Feynman [1]. It is based on the idea of engineering the Hamiltonian of an experimentally controllable quantum system, such that its dynamics can be used as a proxy to understand the physics of seemingly unrelated models that are encoded within it. Such a construction is, in fact, so flexible that it not only provides insight into condensed matter systems, but also into systems of relevance to cosmology and high-energy physics. In recent years, the spectacular advances in experimental techniques facilitating a high degree of control and manipulation of atoms has led to the emergence of cold‐atom experiments as a versatile platform for realizing such quantum simulators.

One such experiment is hosted within our own **Bose-Einstein condensate** (BEC) lab, wherein, thousands of Rb87 atoms are cooled down to the order of micro-Kelvins such that a new phase of matter emerges (i.e., a BEC) that is fundamentally quantum in nature. Such a phase arises from the sudden condensation of all the atoms into a collective state, resulting in a macroscopic quantum object that can be manipulated with laser spots and magnetic fields. This experimental effort was originally initiated in 2022 and we are now ready to start with the first original experiments. A particularly powerful feature of the setup is its flexible projection system that allows us to 'paint' arbitrary potentials onto the BEC, paving the way to encode Hamiltonians into the system. One possible route to achieve this is by applying a periodically driven external potential on the system, such that the time-averaged dynamics are governed by the encoded Hamiltonian, an approach that is broadly known as **Floquet engineering** [2].

While there exist several techniques for engineering new Hamiltonians, a particularly interesting one involves the manufacturing of **synthetic dimensions** [3]. The basic idea is to introduce a coupling between internal degrees of the system and re‐interpret their behavior as dynamics along an effective spatial dimension. This allows us to then simulate the physics of lattice models using our continuous BEC system. A simple way to realize such a construction is by leveraging the formalism of periodically driven systems as mentioned above, and early attempts at this have been corroborated by experiments as well [4]. As a result, this line of research shows considerable promise in realizing exotic quantum dynamics and is an exciting avenue to pursue, motivated by the access to our very own cold-atom experiment.

[1] Simulating Physics with Computers, Richard P. Feynman, [doi:10.1007/BF02650179](https://vql.cs.msu.ru/Feynman.pdf)

[2] Periodically-driven quantum systems: Effective Hamiltonians and engineered gauge fields, N. Goldman, J. Dalibard, [arXiv:1404.4373](https://arxiv.org/abs/1404.4373)

[3] Hannah M. Price, Tomoki Ozawa, Nathan Goldman, Synthetic dimensions for cold atoms from shaking a harmonic trap, [arXiv:1605.09310](https://arxiv.org/abs/1605.09310)

[4] Bloch oscillations along a synthetic dimension of atomic trap states, C. Oliver, et. al., [arXiv:2112.1064](https://arxiv.org/abs/2112.1064)

#### Goal

Initial attempts at manufacturing synthetic dimensions involve rather simple approaches such as the periodic driving of a linear-gradient potential on a non-interacting BEC system [4]. The effects of including interactions as well as the capabilities of more carefully constructed driving schemes remains unexplored.

The goal of this thesis is to understand and develop one such novel periodic driving scheme to engineer a non-trivial lattice Hamiltonian, with a focus on realizing it in our BEC setup. This will involve experimenting with various driving schemes and identifying relevant observables and their experimental signatures that can be detected in our setup. To begin with, the student will familiarize themselves with the formalism of Floquet dynamics of periodically driven systems. This will enable them to formulate theoretically-motivated driving potentials and study their dynamics through numerical simulations of the Gross-Pitaevskii equation using existing software libraries. An ambitious student may also attempt to augment their schemes to mitigate certain unwanted effects, such as the micro-motion [2] resulting from Floquet driving.

As such this thesis consists of **a blend of theory and numerical work in the context of quantum physics, in combination with the unique opportunity to collaborate on a cutting-edge cold atom experiment**. Depending on the interest and skill of the student the topic can be oriented more towards theory, more towards numerics or more towards the actual experiment.  

<p align="middle">
  <img alt="BEC transition" src="/images/thesistopics/2024/CTanghe4.gif" width="300px" />
</p>

