---
title: "A Tensor Network approach to Quantum Repeaters"
promoter: Frank Verstraete
supervisor: Kevin Vervoort
contact: Kevin Vervoort
topic: "Quantum Information"
year: "2024"
---

#### Context

New quantum technologies like quantum key distribution, quantum computation and quantum sensing are nowadays a hot topic. The main ingredient for many of these new technologies is quantum entanglement. By exploiting the sometimes counter-intuitive properties of quantum mechanics, one can do many things that is impossible for a classical computer or system. For example when two distant parties have a source of maximally entangled pairs one can create a secure communication line, which is highly attractive for our current global digital world.

The main difficulty to practically implement these quantum technologies is the creation of entanglement over long distances. Due to decoherence and attenuation one cannot easily create an entangled qubit pair and send it over to the different parties. To overcome this obstacle one can use a quantum repeater. Instead of trying to create the entanglement between two parties in one go, one can first try to establish entanglement between the parties and a trusted node. This trusted node or quantum repeater is situated at the midpoint between the two parties. After the quantum repeater is entangled with both parties it performs an entanglement swapping protocol to establish the long range entanglement between the two parties. The principle of a quantum repeater looks straightforward, but it is notoriously hard to implement due to imperfect measurements and noise.

The framework of tensor networks finds its origin in the field of quantum information and provides the ideal language to study entanglement. Furthermore it allows for a plethora of numerical tools to perform simulations of quantum mechanical systems. One particular instance of tensor networks are matrix product states (MPS). These MPS form a variational class of quantum states for one dimensional systems. MPS are very succesful in capturing the groundstates of many different spin chains. One way to construct such an MPS is by considering different 'virtual' pairs of maximally entangled particles. Then we can perform local projections to project these pairs to a 'physical' particle level. This construction is called the projected entangled pairs construction. In the case of 1D systems this construction is very reminiscent of a quantum channel made out of quantum repeaters. This is the central starting point of the thesis subject.

<p><img alt="A Quantum Repeater Scheme" src="/images/thesistopics/2024/KVervoort1.png" style="float:right; width:500px" /></p>

#### Goal

The overall goal of the thesis is to study and explore quantum repeaters by using tensor networks. The first part of the thesis consists of a literature study on quantum repeaters and quantum entanglement distillation. Secondly the student tries to form a tensor network description of a quantum repeater. For this goal the construction of a MPS from projected entangled pairs will be a good starting point. The student can investigate, by using this tensor network description, which quantum repeater protocols are more optimal. Lastly the student can also investigate the effect of noise and imperfect measurements on the protocols. Depending on the interest of the student one can also look at how to perform entanglement distillation with MPS. Here the student can investigate what measurements are optimal to extract maximally entangled pairs from multiple copies of a MPS.

[1] J. I. Cirac, D. Pérez-García, N. Schuch, F. Verstraete, [arXiv:2011.12127](https://arxiv.org/abs/2011.12127)

[3] K. Azuma, et al., [arXiv:1309.7207](https://arxiv.org/abs/1309.7207)

[3] K. Azuma, et al., [arXiv:2212.10820](https://arxiv.org/abs/2212.10820)


