---
date: "2022-01-28T13:00:00"
speaker: "Pan Zhang"
affiliation: "Institute of Theoretical Physics, Chinese Academy of Sciences"
title: "Simulation of the Sycamore quantum circuits with tensor networks"
type: "lunchtalk"
abstract: true
---

The sampling problem of deep quantum circuits has been proposed recently as a specific computational task to demonstrate whether programmable quantum devices are able to surpass the ability of classical computations, also known as quantum supremacy (or quantum advantage). In 2019, Google released the Sycamore quantum circuits which contain 53 qubits and 20 cycles of unitary operations. Google has demonstrated that the noisy sampling task with fidelity of about 0.002 can be achieved experimentally using the quantum hardware in about 200 seconds, while it would cost 10, 000 years on modern supercomputers.

In this talk, I will introduce two tensor-network methods targeting the sampling problem of the Sycamore circuits. The first method computes amplitudes and probabilities for a large number of correlated bitstrings. The obtained results verify the Porter-Thomas distribution of the large and deep quantum circuits of Google and can be used for spoofing the linear cross entropy benchmark of quantum supremacy using a post-sampling approach. The second method can be used to generate one million uncorrelated bitstrings which are sampled from a final distribution of the Sycamore circuit with 53 qubits and 20 cycles. With the approximate state having fidelity of roughly 0.0037. The whole computation has cost about 15 hours on a computational cluster with 512 GPUs. If our algorithm could be implemented with high efficiency on a modern supercomputer with ExaFLOPS performance, we estimate that ideally, the simulation would cost a few dozens of seconds, which is faster than Google's quantum hardware.

References:
arXiv:2103.03074 (PRL 128, 030501)
arXiv:2111.03011
