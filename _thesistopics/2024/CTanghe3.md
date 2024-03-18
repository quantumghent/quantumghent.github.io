---
title: "Holographic light shaping for quantum simulation"
promoter: Karel Van Acoleyen
supervisor: Clara Tanghe
contact: Clara Tanghe
topic: "Bose-Einstein condensate as a quantum simulator"
year: "2024"
---

#### Context

“Nature isn't classical, dammit, and if you want to make a simulation of nature, you'd better make it quantum mechanical, and by golly it's a wonderful problem, because it doesn't look so easy.” The new blooming field of **quantum simulation** [1] is turning these memorable words of Feynman, uttered more than 40 years ago, into reality. It is based on the idea of engineering the Hamiltonian of an experimentally controllable quantum system, such that its dynamics can be used as a proxy to understand the physics of seemingly unrelated models that are encoded within it. Such a construction is, in fact, so flexible that it not only provides insight into condensed matter systems, but also into systems of relevance to cosmology and high-energy physics.

In recent years, the spectacular advances in experimental techniques facilitating a high degree of control and manipulation of atoms has led to the emergence of cold‐atom experiments as a versatile platform for realizing such quantum simulators. One such experiment is hosted within our own **Bose-Einstein condensate** (BEC) lab, wherein, thousands of Rb87 atoms are cooled down to the order of micro-Kelvins such that a new phase of matter emerges (i.e., a BEC) that is fundamentally quantum in nature. Such a phase arises from the sudden condensation of all the atoms into a collective state, resulting in a macroscopic quantum object that can be manipulated with laser spots and magnetic fields. This experimental effort was originally initiated in 2022 and we are now ready to start with the first original experiments.

The crucial part of the set-up that gives us the finest control both in space and in time is the laser projection system that allows us to shape the light-field that interacts with the atoms. This system is based on Acousto Optical Deflectors (AOD), see for example Ref [2] where they consider attractive light fields.

The AODs contain a crystal whose refractive index can be altered via perturbing it with a sound wave. This creates effectively a diffraction grating for a light beam that passes through this crystal. By programming a simple sinusoidal waveform into the crystal, the diffraction angle of the light can be adjusted. Using different frequencies in the sine wave, this diffracts the light beam in different deflection angles. However, recently a new promising approach emerged for programming optimal diffraction gratings into the AODs, based on the holographic framework. This approach comprises of a more advanced description of the complete light field in terms of changes in amplitude and phase, see Ref [3].

<p align="middle">
  <img alt="ProjectionSystem" src="/images/thesistopics/2024/CTanghe2.png" width="300px" />
  <img alt="Projected UGent logo" src="/images/thesistopics/2024/CTanghe3.jpg" style="float:right; width:300px" />
</p>

[1] Simulating Physics with Computers, Richard P. Feynman, [doi:10.1007/BF02650179](https://vql.cs.msu.ru/Feynman.pdf)

[2] Precise shaping of laser light by an acousto-optic deflector, D. Trypogeorgos, et al., [arXiv:1307.6734](https://arxiv.org/abs/1307.6734)

[3] Artifact-free holographic light shaping through moving acousto-optic holograms, D. Treptow, et al., [doi:10.1038/s41598-021-00332-4](https://doi.org/10.1038/s41598-021-00332-4)

#### Goal

The goal of this thesis is to study and engineer the holographic method unto our AODs with the aim to create specific target potentials, thereby further developing our system towards a full-fledged quantum simulator. As such, the student has the opportunity to **develop and apply numerical methods and quantum optics theory on a cutting-edge quantum experiment**.

The student will start by familiarizing themselves with the workings of an AOD and with the theory of the holographic method on these components. Studying which algorithms, e.g. the Gerchberg-Saxton algorithm, can be adapted to the usage in our system to optimize the information of the target potential into the encodings of the AODs. Then the student will implement the holographic method on the system and compare with the naïve deflection angle method. This encompasses writing code to program the sound wave into the AODs, and taking and analyzing the resulting data of the projected potential. Depending on the interest of the student, machine learning tools such as  neural networks, can be applied to improve the light shaping in an automated fashion.

<p align="middle">
  <img alt="BEC transition" src="/images/thesistopics/2024/CTanghe4.gif" width="300px" />
</p>