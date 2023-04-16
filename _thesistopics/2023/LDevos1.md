---
title: "Contraction ordering of tensor networks in quantum simulation: lessons from the Google Sycamore experiment"
promoter: Jutho Haegeman
supervisor: Lukas Devos
contact: Lukas Devos
topic: "Computational Quantum Many-Body Physics"
year: "2023"
---

#### Context

Tensor networks are an important tool for dealing with high-dimensional quantum systems in condensed matter physics and quantum field theory. They allow us to represent complex wave functions in terms of simple building blocks, and to compute properties of the system efficiently. However, a key bottleneck in tensor network algorithms is the choice of contraction order, which can greatly affect the speed and accuracy of the computation. There are many different possible contraction orders, and finding the optimal one is generally a difficult and time-consuming task.

The Google Sycamore circuit is a quantum computer consisting of 53 qubits that was used to claim quantum supremacy in 2019, by completing a task that Google claimed would take a state-of-the-art supercomputer 10.000 years to finish \[1\]. Nevertheless, through a tensor network algorithm, it was shown that even on a small computational cluster the results were classically reproducible \[2\]. The success of this experiment demonstrated the potential of tensor networks as a tool for quantum simulation, and highlighted the importance of optimizing contraction orders for efficient and accurate computations.

<div align="center">
![Contracting a Tensor Network](/images/thesistopics/2023/LDevos1-1.gif)
</div>

#### Goal

The goal of this master thesis is to investigate the use of reinforcement learning algorithms to optimize the contraction order of tensor networks, with a focus on applications in quantum simulation. Reinforcement learning is a type of machine learning that involves training an agent to take actions in an environment in order to maximize a reward signal. In the context of tensor networks, the agent would be tasked with choosing which pairs of tensors to contract first, and the reward signal would be some measure of the efficiency or accuracy of the resulting contraction. The thesis would involve implementing and testing different reinforcement learning algorithms on a variety of tensor networks, including those used in the Google Sycamore experiment, and comparing their performance to traditional contraction ordering methods. The ultimate aim would be to develop a new approach that can outperform existing methods and lead to faster and more accurate computations of quantum systems. The work proposed in this master thesis could build upon the lessons learned from the Sycamore experiment and further advance the development of tensor network algorithms for quantum simulation.

\[1\] Arute, Frank, Kunal Arya, Ryan Babbush, Dave Bacon, Joseph C. Bardin, Rami Barends, Rupak Biswas, et al. 2019. “Quantum Supremacy Using a Programmable Superconducting Processor.” Nature 574 (7779): 505–10. [https://doi.org/10.1038/s41586-019-1666-5](https://doi.org/10.1038/s41586-019-1666-5).

\[2\] Pan, Feng, and Pan Zhang. 2021. “Simulating the Sycamore Quantum Supremacy Circuits.” ArXiv:2103.03074 [Physics, Physics:Quant-Ph], March. [http://arxiv.org/abs/2103.03074](http://arxiv.org/abs/2103.03074).
