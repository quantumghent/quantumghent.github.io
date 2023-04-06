---
title: "Machine learning for Bose-Einstein condensates"
promoter: Karel Van Acoleyen
supervisor: Karel Van Acoleyen, Clara Tanghe
contact: Clara Tanghe
topic: "Bose-Einstein condensate as a quantum simulator"
year: "2023"
---

#### Context

In spring 2022 we have launched the first Belgian Bose-Einstein condensate (BEC) experiment at UGent. Worldwide such cold atom experiments are currently leading the way in our explorations of the quantum realm.
In summary, a BEC consists of >10.000 bosonic atoms (Rb87 in our case) that are cooled to temperatures T<1 microKelvin. At these temperatures a new phase of matter emerges, the so called Bose-Einstein condensate, with all the atoms condensed into one coherent quantum state.
The spectacular advances in controlling and manipulating the cold BEC atoms allow the experimental realization of many different exotic quantum phenomena like quantum tunneling, superfluidity and quantum non-equilibrium physics.

The generation, manipulation and imaging of a BEC requires many components -coils, drivers, lasers, shutters, cameras– that each need to perform specific actions at specific times. As such one can compare a BEC system to an orchestra where, to produce a symphony, every instrument has to play the right tune at the right instance. While our instrumental control system can perform the required timed actions, the challenge is to find optimal ‘scores’, or in this case ‘recipes’, leading to robust BECs.

The first milestone of creating a BEC in our lab was achieved by starting from rough theoretical predictions, continuing with manually adapting individual component values, to find an "apparent" optimum for BEC.
This is very time-consuming and the interplay between multiple parameters could be missed. In contrast, machine learning techniques have been proven to give better results than what was found manually in the same systems, yielding larger atom clouds with better fractions of number of condensed atoms over thermal atoms [1,2].

<p align="middle">
  <img alt="Science chamber" src="/images/thesistopics/2023CTanghe1.png" width="300px" />
  <img alt="BEC transition" src="/images/thesistopics/2023CTanghe2.gif" width="300px" />
  <img alt="ML cost example" src="/images/thesistopics/2023CTanghe4.png" style="float:right; width:300px" />
</p>

From left to right:

- Picture of the science chamber containing a cloud of fluorescing atoms with temperatures around a few hundreds microKelvin.

- Images of an atom cloud that is cooled down by evaporating further and further (lowering the RF5-parameter). The onset of condensation is visible when a tight ellips of condensed atoms appears within the round distribution of thermal atoms. Evaporating even further, also condensed atoms are expelled from the trap.

- Example of iteratively changing a parameter in the evaporation procedure and the resulting cost-function-value (here: center amplitude of an atom cloud).

#### Goal

The goal of this thesis is to develop and study numerical optimization sequences that will lead to ideal BECs for our system, helping us to achieve high-quality BECs in a robust manner.

The instrument control system can be commanded via a python script that runs optimization code.
There is a lot of flexibility to encode protocols driven by self-defined cost-functions. Different experimental scenarios will call for different BEC-benchmarks, such as number of atoms in the cloud, condensation fraction, how fast is a BEC created, etc. An objective is to find which cost function and/or machine learning protocol is best suited for which scenario, while looking at the dependencies on key components in the set-up. By letting the program learn a model about our system, insight could be gained into the deeper underlying physics of the experiment.

This thesis will give the student the opportunity to apply and develop machine learning techniques on a state-of-the-art ultra-cold atom experiment.

[1] A.J. Barker, H. Style, K. Luksch, S. Sunami, D. Garrick, F. Hill, C.J. Foot, E. Bentine, Applying machine learning optimization methods to the production of a quantum gas, Machine Learning: Science and Technology. 1, 015007, (2020), [arXiv:1908.08495](https://arxiv.org/abs/1908.08495).

[2] Z. Vendeiro, J. Ramette, A. Rudelis, M. Chong, J. Sinclair, L. Stewart, A. Urvoy, and V. Vuletić, Machine-learning-accelerated Bose-Einstein condensation, Phys. Rev. Research. 4, 043216, (2022), [arXiv:2205.08057](https://arxiv.org/abs/2205.08057).
