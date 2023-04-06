---
layout: thesistopic
title: "Quantum control theory for Bose-Einstein condensates"
promoter: Karel Van Acoleyen, Alain Sarlette
supervisor: Karel Van Acoleyen, Clara Tanghe
contact: Clara Tanghe
topic: "Bose-Einstein condensate as a quantum simulator"
year: "2023"
---

#### Context

In spring 2022 we have launched the first Belgian Bose-Einstein condensate (BEC) experiment at UGent. In summary, a BEC consists of >10.000 bosonic atoms (Rb87 in our case) that are cooled to temperatures T<1 microKelvin.
At these temperatures a new phase of matter emerges, the so called Bose-Einstein condensate, with all the atoms condensed into one collective quantum state.
The unique feature of cold atom experiments such as ours is the high level of control: carefully tuned electromagnets and lasers provide many ‘knobs’ for manipulating the BEC and thereby realizing new experiments that can explore different aspects of the quantum realm.

A basis fundamental task, appearing in different experimental protocols, is to evolve a certain initial BEC quantum state into another target state.
One option to achieve this is via adiabatic evolution: by slowly changing the trapping potential the BEC will follow accordingly.
However, time is costly in cold atom experiments - the typical BEC lifetime is one second - so other faster strategies for driving the potential are necessary. It is for this type of problem that control theory can make a big difference.

<p align="middle">
  <img alt="Science chamber" src="/images/thesistopics/2023CTanghe1.png" width="300px" />
  <img alt="Alice and Bob" src="/images/thesistopics/2023CTanghe5.jpg" width="300px" />
  <img alt="Split condensate" src="/images/thesistopics/2023CTanghe6.png" width="300px" />
 </p>

#### Goal

The goal of the thesis is to study and apply control theory in the quantum context, in particular in the context of BEC physics, see e.g. [1].
A specific quantum control task that we have in mind involves the coherent splitting of the BEC in two separate clouds (A and B), with a particular relative complex phase between the clouds. This relative phase can be interpreted as a piece of quantum data that is hidden in the correlation between A and B (see [2]), which can only be read out by looking at the interference patterns that emerge in time of flight images. The aim then is to design the optimal driving protocols that allow for maximal control on this relative phase. On the one hand this will entail numerical simulations of the famous Gross-Pitaevskii equation (with existing numerical packages), that can describe the evolution of the BEC state under different driving conditions. On the other hand, the plan is also to test optimized driving protocols that come out of this numerical work in the actual experiment.

As such this thesis consists of a blend of theory and numerical work in the context of quantum physics and quantum information, in combination with the unique opportunity to collaborate on a cutting-edge cold atom experiment.
Depending on the interest and skill of the student the topic can be oriented more towards theory, more towards numerics or more towards the actual experiment.

[1] Optimal control of complex atomic quantum systems, S. van Frank, M. Bonneau, J. Schmiedmayer, S. Hild, C. Gross, M. Cheneau, I. Bloch, T. Pichler, A. Negretti, T. Calarco, S. Montangero, [arXiv:quant-ph/0302039](https://arxiv.org/abs/1511.02247)

[2] Quantum nonlocality in the presence of superselection rules and data hiding protocols, F. Verstraete, J.I. Cirac, [arXiv:quant-ph/0302039](https://arxiv.org/abs/quant-ph/0302039)
