---
title: "QuantumGroup@UGent - Master thesis"
layout: textlay
excerpt: "QuantumGroup@UGent -- Master thesis topics"
sitemap: false
permalink: /studentinfo/thesis.html
---

<h1>Master thesis topics of the Quantum Group @ UGent</h1>

<hr><h2>Classical supremacy</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Maarten Van Damme</td></tr>
</tbody></table>

<h3>Context</h3>
<p>It is astounding just how much progress has been made in the field of quantum computing during the last decade. Billions have been invested, but the results are there. Both IBM and Google can do computations with upwards of 50 qubits, well beyond the reach of your average comuptational cluster. In fact, a 2019 paper appears to demonstrate that this is the era of quantum supremacy, by doing a computation that we cannot do on a classical computer. The researchers estimated that simulating the full circuit would take 10,000 years even on a computer with one million processing units (equivalent to around 100,000 desktop computers).</p>

<p>But is that really so? The quantum computer used was far from perfect, with the final precision estimated at 0.2%. While a perfect simulation may be unfeasable on desktop pc, maybe we can also allow for noise in a clever way, allowing us to reach a similar precision.</p>

<h3>Goal</h3>
<p>In this proposal we hope to reclaim - or at least try to reclaim - supremacy of the classical computer using tensor network techniques. The faithfull simulation of the "quantum supremacy circuit" can be represented as one big tensor network contraction, which we will try to do approximately. Such an algorithm would also be useful for statistical mechanics: partition functions can usually be written as a tensor network.</p>

<hr><h2>Continuous tensor network states for inhomogeneous systems</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete, Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Benoît Tuybens, Bastiaan Aelbrecht</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Many of the low dimensional strongly interacting systems of current interest, such as the ones realized in cold atom experiments, are not described by lattices but&nbsp;rather by continuum field theories. Rather than discretizing&nbsp;the field theory (hereby introducing cut-off effects) and using lattice techniques, there exists a particular family of variational trial states, known as continuous matrix product states (cMPS), that can directly parameterize wavefunctions in the continuum. The cMPS ansatz is a direct generalization of the extremely successful matrix product state, which has become the de facto standard technique for studying spin systems, but has emerged in various other disciplines of physics, chemistry and mathematical engineering (where they are known as tensor trains), including for machine learning applications. Since their conception in 2010, the&nbsp;cMPS ansatz&nbsp;has been successfully applied to some continuous condensed matter hamiltonians, but when applying the time dependent variational principle (TDVP) to the cMPS manifold [1], a non-trivial matrix-valued partial differential equation emerges, which so far has resisted any integration attempt. With this in mind, a new method was created which has its roots in finite elements analysis (a linear interpolation of the matrices in the ansatz). This recently developed method [2] has so far only been applied to find ground states of a non-relativistic (Lieb-Liniger) Hamiltonian.</p>

<p>[1] Jutho Haegeman, Damian Draxler, Vid Stojevic, J. Ignacio Cirac, Tobias J. Osborne, Frank Verstraete. Quantum Gross-Pitaevskii Equation. https://arxiv.org/abs/1501.06575</p>

<p>[2] Benoit Tuybens, Jacopo De Nardis, Jutho Haegeman, Frank Verstraete. Variational optimization of continuous matrix product states. https://arxiv.org/abs/2006.01801</p>


<h3>Goal</h3>
<p>There are many obvious ways in which these preliminary results can be extended, giving rise to some flexibility for the student to steer this thesis project in his/her preferred direction.&nbsp;In particular; it is possible to explore how cMPS algorithms can be used to simulate realistic higher-dimensional quantum many body systems, either ones that are confined in two directions such as in cold atom experiments (for this, it will be enough to describe the modes as particles in the cMPS ansatze), or systems with a spherical symmetry, in which the cMPS would represent the radial part of the wavefunction (and angular components again appear as different modes).</p>

<p>We have in-house code available for working with inhomogeneous cMPS, that would need to be adapted to deal with those new settings. Furthermore, our group is also setting up a BEC experiment, such that the simulations in this project could be targetted to have direct experimental relevance and impact.</p>

<hr><h2>Generative machine learning with PEPS tensor networks</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete, Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Tom Vieijra, Benoît Tuybens</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Since the invention of the density matrix renormalization group (DMRG), tensor networks have become an increasingly powerful class of techniques to characterize quantum many-body systems.&nbsp; Motivated by this success, algorithms typically used for studying many-body physics have found their way to other contexts, one of which machine learning.&nbsp; More specifically, the link between describing a vector in an exponentially large Hilbert space (e.g. finding the ground state of a quantum hamiltonian with tensor networks) and finding the probability distribution described by a data set where every sample can be seen as a basis state in a high-dimensional vector space is striking.&nbsp; These links led to the use of matrix product states for supervised and unsupervised machine learning, as well as the use of tree tensor networks and projected entangled pair states (PEPS) for supervised classification tasks.</p>

<p>In this thesis, we will look at unsupervised problems in two dimensions, e.g. the generation of novel data samples according to the probability distribution given by a data set.&nbsp; Typical data sets are pictures of handwritten digits (MNIST) or pictures of clothing objects (Fashion-MNIST), which have been studied very extensively and for which many benchmarking results are readily available.&nbsp; Our aim is to use 2D tensor networks such as PEPS to describe the probability distrubution of the data sets and generate new samples according to it.&nbsp; Generation of data samples requires an efficient way of sampling from a probability distrubution, for which our research group developed new techniques.</p>

<h3>Goal</h3>
<p>The scientiffic work for this thesis will consist of a literature study of the specific literature around machine learning with tensor networks, as well as literature concerning tensor networks techniques in a physical context.&nbsp; Afterwards, the aim is to develop a generative algorithm for data.&nbsp; First we will focus on&nbsp;a 1D tensor network as a case study and as a benchmark for our novel algorithm based on 2D tensor networks.&nbsp;&nbsp;Then, we will focus on&nbsp;2D tensor network to study in which sense it has performance advantages over the 1D models and other generative machine learning models such as neural networks or Boltzmann machines.</p>

<hr><h2>Non-local correlators in critical spin systems</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Laurens Lootens, Robijn Vanhove</td></tr>
</tbody></table>

<h3>Context</h3>
<p>In 2-dimensions, many real systems can be studied using simple models in statistical mechanics, an example being the 2D Ising model for a ferromagnet. On of the most striking features of these models is that they can undergo a phase transition where the system becomes critical and scale invariant. In the continuum limit, such phase transitions are described by conformal field theories, which have been the subject of intense study ever since their conception some 40 years ago, finding application in condensed matter physics, string-theory and the AdS/CFT correspondence to name just a few. Despite steady progress, the exact relation between lattice observables and their continuum counterparts is still rather poorly understood. In fact, the almost 100-year old 2d Ising model was only rigorously shown to correspond to the Ising CFT in the continuum limit some 10 years ago by Smirnov, in a work which netted him the Fields Medal in 2010. Understanding this correspondence for more general models is important because knowing the continuum limit of some lattice operator allows us to exactly predict its long-range behaviour, since this is completely dictated by the CFT. One particularly poorly understood aspect are operators that have some non-local aspect to them, for example the observables at the endpoint of some lattice dislocation.<br>
<br>
<img alt="2d Ising model at the critical point, exhibiting scale invariance" src="{{ site.url }}{{ site.baseurl }}/images/thesis/A-critical-Ising-model-Black-and-white-represent-1-spins-The-cluster-boundaries_W640.jpg" style="height:429px; width:429px"></p>

<h3>Goal</h3>
<p>In the quantum group in Ghent, we have developed a novel way of interpreting critical lattice models. Our approach is based on tensor network descriptions of systems with topological order, which require the presence of non-local symmetries called matrix product operators (MPOs). These MPO symmetric tensor networks turn out to be exactly the right language for studying critical lattice models as well, a result which can be understood from the field theory point of view as a lattice version of the holographic duality between topological and conformal field theories. The various operators in the statistical mechanics model can be understood using the language of MPO symmetries, and from this point of view, non-local operators at e.g. lattice dislocations pose no difficulties whatsoever. Predictions made based on this ansatz can numerically be verified using the powerful tensor network toolbox developed in our group, which is at the cutting edge of this type of research. The student is expected to familiarize themselves with both the theoretical construction of critical lattice models from topologically ordered systems, as well as the numerical component of calculating observables in tensor networks. The latter requires a firm grasp of the underlying linear algebra, and a good knowledge of the algorithms we use to solve eigenvalue problems in this specific setting.</p>

<hr><h2>Painting potentials on a Bose-Einstein condensate &nbsp;</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Karel Van Acoleyen, Kasper Van Gasse</td></tr><tr><td>Begeleider(s):</td><td></td></tr>
</tbody></table>

<h3>Context</h3>
<p>In 2021 we will start up the first Belgian Bose-Einstein condensate (BEC) experiment at UGent (within the quantum group, in collaboration with the photonics department). Worldwide such cold atom experiments are currently leading the way in our explorations of the quantum realm. In summary, a BEC consists of &gt;10.000 bosonic atoms (Rb87 in our case), that are cooled to temperatures T&lt;1 microKelvin. At these temperatures a new phase of matter emerges, the so called Bose-Einstein condensate, with all the atoms condensed into one coherent quantum state. As such, BECs allow the experimental realization of many different exotic quantum phenomena like quantum tunneling, superfluidity, or even the quantum simulation of black holes.</p>

<p>The cooling, trapping, and manipulation of the atoms relies on both magnets (through the Zeeman effect) and lasers (through the dipole-interaction). In particular our BEC set-up uses a state-of-the-art combination of magnetic fields generated by an atom chip and a laser projection system that operates with an Accousto Optical Deflector (AOD). With the latter system we will be able to 'paint' flexible (both in space and time) potentials on the atom cloud, allowing for new original BEC experiments. It is also this latter system that is the subject of this thesis.&nbsp; &nbsp; &nbsp;&nbsp;</p>

<h3>Goal</h3>
<p>The goal of this thesis is to study and develop optimal protocols for driving the AOD, in function of the specific potentials in the atom cloud that we want to realize with our set-up.</p>

<p>In short, an AOD relies on the accousto optical effect, which amounts to an effective interaction between sound waves and light within certain crystals. By driving the AOD with ultra-sonic sound waves, the laserbeam is deflected in a direction that depends on the sound frequency. Upon projection through two microscopes, this beam direction in the end translates to a position of a laser spot on the atom cloud.</p>

<p>For finding the optimal driving protocols there are two different, yet very much connected aspects that will have to be studied. First there is the issue of the driving itself, where one has the option to drive the AOD with a single frequency, resulting in one spot at at time, or with a superposition of multiple frequencies resulting in multiple spots at the same time. The second issue is the effect on the atom cloud, where the idea is to generate effective time-averaged potentials by scanning one or multiple spots very fast through the cloud.</p>

<p>The work on this thesis will require a combination of photonic physics, numerical simulation, quantum theory, and experimental cold atom physics. Depending on her/his interests, the student will have the freedom to focus more on particular aspects of the problem.</p>

<hr><h2>Percolation as  a tensor network</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete, Romain Couvreur</td></tr><tr><td>Begeleider(s):</td><td>Laurens Lootens</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Percolation theory is an important tool to analyze many natural phenomena such as disease outbreaks, propagation of fires, porous media (hydrocarbon reservoirs, biological tissues) or even traffic models. From a more fundamental point of view, percolation is also an important toy model to understand many stochastic processes, universality features and the Renormalisation Group in statistical field theory. In two dimensions, a percolation configuration on a square lattice can be obtained as follows: each edge is independently considered filled (closed) with a probability p&nbsp;and empty (opened) with a probability 1-p. If p&nbsp;is larger than a particular value p_c&nbsp;(the percolation threshold), a path connecting two opposite sides of the system exists. As a consequence, a fluid or an electrical current is able to propagate across the system. We say that the system percolates. A second order phase transition exists at p=p_c, the system is critical and scale invariant. In the continuum limit (or large size limit), it is described by a conformal field theory with many interesting features (non-unitary, non-rational, logarithmic). Using algebraic techniques, it is possible to calculate the critical exponents exactly. These are universal and do not depend on the microscopic details of the system (like the exact shape of the lattice).&nbsp;<br>
Tensor networks, which were introduced for their efficient representation of quantum many body systems, also provide a conceptually transparent and computationally efficient representation of such statistical models. The methods developed in our group for computing with these tensor networks result in powerful numerical algorithms to tackle new problems.</p>

<h3>Goal</h3>
<p>In this project, we propose to first build a tensor network representation of percolation. The student will compute numerically correlation functions and the critical exponents of 2d percolation. Depending on the student's main interest, different topics, analytical or numerical, can be pursued. We propose to map the mentioned tensor network model to a quantum spin chain. The student will investigate the entanglement properties, look for symmetries and compare with other supersymmetric models of percolation. From a numerical point of view, the student will be encouraged to use state-of-the-art tensor network algorithms to compute correlation functions and improve results obtained with standard Monte-Carlo techniques.</p>

<hr><h2>Polarons in strongly-correlated electron systems: a proxy for high-Tc superconductivity</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Laurens Vanderstraeten, Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Maarten Van Damme</td></tr>
</tbody></table>

<h3>Context</h3>
<p>High-temperature superconductivity constitutes one of the big open questions in contemporary physics. From the experimental side, realizing high-temperature superconductivity in realistic materials remains one of the holy grails of experimental condensed-matter physics. From the theoretical side, a thorough understanding of the physical mechanism behind high-Tc superconductivity is still lacking, and revolves around the most central questions in strongly-correlated quantum many-body physics. One route towards a better understanding is via numerical simulations of simplified models such as the Hubbard model, which, despite its apparent simplicity, contains all ingredients for exhibiting superconductivity (and many more exotic many-body effects). Indeed, the Hubbard model is paradigmatic in realizing the ideal of emergence: very simple microscopic interactions can lead to a plethora of interesting collective effects, that cannot be understood on the microscopic level alone and, therefore, need new physical concepts that function on the macroscopic level.</p>

<p>In this master thesis, we investigate the properties of charge carriers in the Hubbard model on the triangular lattice. It has been realized recently that these eletronic "holes" are, in fact, composite objects that can only exist on a strongly-correlated background. Indeed, these so-called polarons consist of a chargeon and spinon, two new emergent quasiparticles that have fractional quantum numbers. It was conjectured that the non-trivial polaron properties are, in fact, responsible for the hole pairing causing superconductivity. Investigating the properties of these polarons with numerical techniques is of paramount importance for making this conjecture more tangible, and moving forward in understanding high-Tc superconductivity.</p>

<p>References:<br>
[1] J. Vijayan, et al, Time-resolved observation of spin-charge deconfinement in fermionic Hubbard chains, Science 367,186 (2020)<br>
[2] A. Bohrdt, et al, Classifying snapshots of the doped Hubbard model with machine learning, Nature Physics 15, 921 (2019)<br>
[3] A. Bohrdt, Parton theory of angle-resolved photoemission spectroscopy spectra in antiferromagnetic Mott insulators, Physical Review B 102, 035139 (2020)</p>

<h3>Goal</h3>
<p>In this master thesis, we will numerically simulate the polaron problem in the triangular-lattice Hubbard model. For that goal, we will use the formalism of tensor network -- a formalism that was invented by the senior researchers in our group. We will apply a method that was recently developed by the group [1] for simulating low-energy excitations on top of the ground state. Using this method, we can determine the dispersion relation of the polaron and look at the "quasiparticle weight" of this state. Next, having a variational wavefunction for this state, we can investigate the composite nature of the polaron, and investigate the confining force between the chargeon and the spinon.</p>

<p>The thesis, therefore, involves writing performant computer codes, numerical simulations and interpretation of the numerical results. The latter will involve a thorough understanding of the relevant literature and the open questions in the field.</p>

<p>[1] M. Van Damme, et al, Efficient MPS methods for extracting spectral information on rings and cylinders, arXiv 2102.10982</p>

<hr><h2>Pursuing the fractional quantum Hall effect with tensor networks</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Laurens Vanderstraeten, Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Quinten Mortier</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Take a thin planar conductor, let a current run through it and apply a strong orthogonal magnetic field. This simple setup provides the setting for one of the most remarkable condensed-matter phenomena discovered in the second half of the 20th century, the quantum Hall effect. Its most striking and experimentally most visible feature is the organization of the transverse Hall conductivity&nbsp;in plateaus labeled by an integer. I.e. also macroscopic quantities like resitivities, depending on many particles, can be quantized. This emergent quantization originates from the interplay between topology and quantum mechanics and has, in contrast to many other properties of condensed-matter systems, no classical analogue. Where the integer nature of the effect&nbsp;was initially reproduced in experiments to an extraordinary precision, Tsui and Störmer discovered in 1982 that in certain systems with reduced (but still non-zero) disorder, the quantum number could also take on rational values. This fractional quantum Hall effect was later understood by Laughlin as originating from the interactions between electrons, resulting in highly correlated quantum states that are nowadays recognized as a new phase of matter. In this fractional quantum Hall phase the charged particles carry a fraction of the electron charge and even the statistics of the charge carriers fractionalizes yielding anyonic behavior.</p>

<p><img alt="" src="{{ site.url }}{{ site.baseurl }}/images/thesis/fqhe.jpg" style="height:217px; width:300px"></p>

<p>Studying the (fractional) quantum Hall effect and more generally quantum many-body physics is greatly complicated by the exponential scaling of the relevant Hilbert space with the number of particles. However, over the last two decades, tensor networks revealed themselves as extremely suitable ansatzes in this context as they can target the physically relevant corner of this Hilbert space to a remarkable degree. In 1d, for instance, Matrix-Product States (MPS) have been applied to a myriad of problems and were even able to classify all 1d topological phases. The construction was also extended to 2d yielding the class of Projected Entangled-Pair States (PEPS) that constitutes a vibrant topic of research to this day.</p>

<h3>Goal</h3>
<p>The main goal of this project is to capture the (fractional) quantum Hall effect by tensor network states for the specific case of the (interacting) Hofstadter model. This model is well-known for the fractal nature of its spectrum, earning it its nickname, "Hofstadter's butterfly", and exhibiting a rich phase diagram with multiple topological phases. A first goal will consists of optimizing the Gaussian and fermionic variant of PEPS for the non-interacting version of the model and deriving its topological properties, essentially "capturing Hofstadter's butterfly". When successful, the model can be extended with interactions and the Gaussian PEPS can be used as a starting point for variational optimization of interacting PEPS (e.g. on a cylinder) to obtain an approximation of the ground state exhibiting the fractional quantum Hall effect.</p>

<p><img alt="" src="{{ site.url }}{{ site.baseurl }}/images/thesis/hof.jpg" style="height:225px; width:300px"></p>

<hr><h2>Quantum algorithms for finding quantum many-body groundstates</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Karel Van Acoleyen, Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Maarten Van Damme</td></tr>
</tbody></table>

<h3>Context</h3>
<p>The spectacular technological advances towards building a quantum computer (e.g. Google’s sycamore) brings the question on useful applications to the forefront. As believed by many in the field, the killer app is going to be the quantum simulation of strongly correlated quantum many body systems. Such systems are ubiquitous in the natural world, ranging from quantum chemistry over condensed matter physics to high energy physics.</p>

<p>An important first step for simulating a quantum many body system, is the simulation (= computation) of its groundstate. This can for instance serve as the starting point for a real-time evolution after a quantum quench, or for creating localized particle excitations (in the context of quantum field theoretic applications) on top of this vacuum groundstate.</p>

<h3>Goal</h3>
<p>The goal of this thesis is to study and explore the so called Quantum Metropolis sampling algorithm for simulating groundstates of quantum many body systems. This algorithm modifies the classical Metropolis sampling for finding thermal states of classical stat-mech systems to the quantum setting, overcoming quantum hurdles like the no-cloning theorem and the irreversibility of the measurement process.</p>

<p>For benchmarking the algorithm, the student can study small size implementations on IBM’s online quantum computer. Furthermore, for larger systems, we want to study the performance of the algorithm in the context of the exactly solvable models, like the quantum Ising model. Important questions that this thesis might shine some light on are: what is the expected performance on the quantum computers in the current so called Noisy Intermediate-Scale Quantum (NISQ) era? Could we transpose ideas from scaling theory, developed for finite size or finite entanglement simulations, towards simulations with finite circuit depth or nonzero gate fidelity?</p>

<p>Depending on the student’s interests and skills the thesis can be oriented more towards theory (e.g. the quantum simulation of quantum field theories) or towards the algorithmic side. There is enough to be done.&nbsp;Also students with a limited physics background can apply.&nbsp; &nbsp; &nbsp;&nbsp;</p>

<hr><h2>Quantum data hiding in a Bose-Einstein condensate</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Karel Van Acoleyen, Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td></td></tr>
</tbody></table>

<h3>Context</h3>
<p>In 2021 we will start up the first Belgian Bose-Einstein condensate (BEC) experiment at UGent. Worldwide such cold atom experiments are currently leading the way in our explorations of the quantum realm. In summary, a BEC consists of &gt;10.000 bosonic atoms (Rb87 in our case), that are cooled to temperatures T&lt;1 microKelvin. At these temperatures a new phase of matter emerges, the so called Bose-Einstein condensate, with all the atoms condensed into one coherent quantum state, that can be controlled and manipulated through the application of magnetic and optical fields.</p>

<p>In this thesis we want to approach BEC physics from the quantum information standpoint. The underlying principle of quantum information is that quantum mechanics allows us to carry certain tasks that would be impossible in a classical world. This becomes especially apparent when natural limitations apply to the allowed operations. Typically this limitation comes from a notion of locality, where two parties (the infamous Alice and Bob) can only perform local quantum operations on their respective subsystems, possibly supplemented with a classical communication channel. This is the standard framework of the so called&nbsp; LOCC protocols, that for instance allow for quantum teleportation and quantum key distribution.</p>

<p>However, in [1] it was realized that additional limitations on the allowed operations can lead to new interesting possibilities. In particular, in many systems of interest we have so called superselection rules. Specifically, in the context of BEC experiments, the superselection rule is that coherent superpositions of states with a different atom number are forbidden. Or equivalently, that all (local or non-local) measurements have to commute with the total atom number. As shown in [1], such an additional constraint allows for perfect data hiding, where some information can be distributed between Alice and Bob, in such a way that they can only read it if they are provided with the means to perform joint measurements.</p>

<p>&nbsp;</p>

<p>[1] F. Verstraete and J.I. Cirac, ' Quantum nonlocality in the presence of superselection rules and data hiding protocols,' Phys. Rev. Lett. 91, 010404 (2003)</p>

<h3>Goal</h3>
<p>The goal of this thesis is to explore the possibility of experimentally realizing a protocol for perfect data hiding on our BEC set-up. For the experiment that we have in mind, Alice and Bob would correspond to two spatially separated BEC clouds that are still coherent. The hidden data can be encoded in the relative phase between the two clouds. While the joined measurement for reading out this data, can be performed by interfering these clouds with a third 'reference cloud'. A main challenge for this experiment will be the control on the trapping potential that in our case is provided by magnetic fields from an atom chip in combination with a highly flexible optical field from a laser projection system.</p>

<p>The student working on this project will the have the opportunity to perform original experiments on a state-of-the-art installation, while at the same time learning about quantum information, optics and cold atom physics.</p>

<hr><h2>Quantum error correction and non-Abelian topological order: from the theory to the lab</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Lander Burgelman</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Quantum computation and quantum information has developed into a rich and highly attractive research field over the past few decades. Though significant progress has been made from both the theoretical and experimental perspective, protecting quantum information from errors due to interactions with the environment remains the central challenge that must be overcome in order to achieve scalable quantum computation. The discovery of quantum error correcting codes in the 1990s already proved that quantum information could indeed be effectively protected from this decoherence. However, the search for an error correction framework that is suitable for near-term experimental implementation still forms one of the most vibrant research topics in physics at this date.</p>

<p>Many of the current leading proposals for fault-tolerant architectures rely on the concept of topological order. This is an exotic type of long-range quantum order that cannot be described in terms of any local order parameter. Topological quantum error correction exploits this phenomenon by encoding quantum information in the global topological properties of a system, which is then inherently protected from local errors. Although these current proposals provide a robust way of storing quantum information, they require an enormous overhead in order to actually process the stored information [1]. A way around this problem is to use codes that possess a more intricate non-Abelian topological order, which allow for universal computation without the need for any additional machinery.</p>

<p>Topological order can be captured in an elegant way using the framework of tensor networks, which has been explored by our group in recent years. Building on these concepts, we have recently proposed a framework for error correction using non-Abelian topological order, and have provided the first-ever numerical demonstration that successful error correction is indeed possible in this setting [2]. However, some important steps must still be taken in order to transform this first proof of concept into a concrete and competitive proposal for an experimental realization of a quantum architecture. This forms the topic of this master's thesis.</p>

<p>[1] Earl T. Campbell, Barbara M. Terhal, and Christophe Vuillot. Roads towards fault-tolerant universal quantum computation. Nature, 549(7671):172–179, September 2017.</p>

<p>[2] Alexis Schotte, Guanyu Zhu, Lander Burgelman, and Frank Verstraete. Quantum error correction thresholds for the universal Fibonacci Turaev-Viro code. arXiv:2012.04610, December 2020.</p>

<h3>Goal</h3>
<p>The goal of this thesis project is to analyze what resources would be required for a minimal working realization of a non-Abelian code, and to investigate its performance. This can be broken down into several parts. The first is a more theoretical one, in which the student will expand on the framework established by the group in order to construct a non-Abelian code that is specifically tailored toward experimental realization using the minimal amount of resources possible. This will involve exploring different code interactions, experimenting with adaptive lattices, and investigating different encodings that allow for a practical geometry. A second aspect will be the numerical simulation of error correction in this adapted code, in order to demonstrate the possibility of successful error correction and to compare the performance of different proposals. Finally, a crucial step will be the translation of a proposed code into a complete framework for an error correction architecture that may be realized in the lab. This will consist of identifying a suitable experimental paradigm currently used for the construction of quantum hardware and synthesizing concrete quantum circuits for all logical and error correction operations required, tailored to the specific hardware technology. At that point, the actual performance of this complete framework could be analyzed using currently available quantum simulators (by IBM, Google, Xanadu and the likes), and it could even lead to a real life realization of the code in a collaboration with an experimental group.</p>

<hr><h2>Quantum simulation of Hawking radiation with a Bose-Einstein condensate &nbsp;</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Karel Van Acoleyen</td></tr><tr><td>Begeleider(s):</td><td></td></tr>
</tbody></table>

<h3>Context</h3>
<p>In 2021 we will start up the first Belgian Bose-Einstein condensate (BEC) experiment at UGent. Worldwide such cold atom experiments are currently leading the way in our explorations of the quantum realm. In summary, a BEC consists of &gt;10.000 bosonic atoms (Rb87 in our case), that are cooled to temperatures T&lt;1 microKelvin. At these temperatures a new phase of matter emerges, the so called Bose-Einstein condensate, with all the atoms condensed into one coherent quantum state. The spectacular advances in controlling and manipulating the cold BEC atoms allow the experimental realization of many different exotic quantum phenomena like quantum tunneling, quantum non-equilibrium physics, superfluidity, and even the quantum simulation of black holes. It is the latter avenue that we want to explore with this thesis.</p>

<p>In 1975 Stephen Hawking publishes his spectacular result on the quantum behavior of black holes. In his paper 'Particle creation by black holes' Hawking demonstrates that the vacuum of a relativistic quantum field theory on a space-time with an event horizon produces radiation. In other words, a quantum black hole is not really black, it emits radiation at a certain Hawking temperature. Unfortunately, for realistic astrophysical black holes this predicted Hawking temperature is orders of magnitudes below the temperature of the cosmic background radiation, eluding experimental detection. And as such the Hawking effect has predominantly been studied purely theoretically, as it seems to offer important clues towards a theory of quantum gravity.</p>

<p>However, in the eighties Bill Unruh advocated that the Hawking effect is universal, in the sense that it can appear in many different other systems. In particular, he realized that the behavior of the large-scale fluctuations of (super)fluids (the phonons) can be mapped to a relativistic quantum field theory (QFT) on a particular space-time, with the space-time metric depending on the (super)fluid velocity. This opened up new possibilities for experimentally realizing the Hawking effect; and BECs indeed seemed the perfect candidate for this. Incidentally, the term 'quantum simulation' in the thesis title denominates precisely the realization of a certain quantum behavior by an experimental quantum system that can be controlled and manipulated.</p>

<h3>Goal</h3>
<p>The goal of this thesis is to study and explore the BEC quantum simulation of a black hole towards actual experiments on our set-up. Notice that in a series of experiments from 2010 till now, Jeff Steinhauer has already been working up to such a feat, with a claimed experimental detection of Hawking radiation in 2017. However, this claim was put in doubt by other physicists. In any case, the thesis fits in the grand goal of replicating and/or improving on these experiments.</p>

<p>For such a BEC analogue black hole experiment we can roughly delineate two steps. First one has to bring the BEC in the supersonic regime, i.e. a regime where the BEC superfluid flows faster than the phonon speed. It is in this regime that the effective black hole metric is realized. The second step then consists of detecting the Hawking radiation. This is found through correlated fluctuations (Hawking pairs) at both sides of the horizon. Notice that in contrast to actual black holes, for a simulated quantum black hole one indeed has access to both sides of the horizon. Experimentally, these correlations are found through the measurement of expectation values, by performing many different (automated) versions of the same experimental protocol. The challenge here is to separate the actual quantum fluctuations, from other fluctuations that are inherent to the experiment.</p>

<p>This thesis draws from different fields: quantum optics, quantum field theory, relativity, numerical analysis and cold atom physics. Of course we don't expect the student to master all these fields. As the thesis fits within a larger research goal of our group, depending on her/his interests and skills the student will have the freedom to focus more on the theoretical, numerical or experimental part of the project.</p>

<hr><h2>Restoring quantum fields</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Karel Van Acoleyen, Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Maarten Van Damme</td></tr>
</tbody></table>

<h3>Context</h3>
<p>"Nature isn't classical, dammit, and if you want to make a simulation of nature, you'd better make it quantum mechanical, and by golly it's a wonderful problem, because it doesn't look so easy.” - Richard Feynman</p>

<p>Strongly interacting quantum systems are difficult. Continuously<br>
strongly interacting systems even more so. It is no long useful to consider some diagramatic perturbation theory and the hilbert space is intractably large for numerical simulations. We have to make simplifications, and one of these is mapping it to a lattice model. Such a lattice model can then be simulated in real life (cold atom experiments, quantum computer, NISQ systems).</p>

<h3>Goal</h3>
<p>After performing the experiment, it's necessary to be able to go back to the continuum model and make quantitive predictions there. In general, there are some obstacles in the way:</p>

<p>- Generically experiments will have some noise. Can we protect against them efficiently? To what extend does this change the measurements results?<br>
- Quantum field theories can have an infinite number of particles in one location, which has to be truncated down to a finite degrees of freedom for numerics/experiments. In what sense can we restore the original theory?<br>
- Some symmetries cannot survive the transition to a lattice model, but one would still expect to see remnants at low momenta. How do these manifest themselves?</p>

<p>In this project we would try to answer those kind of questions using a mix of analytical and numerical techniques.</p>

<hr><h2>Simulating the Heisenberg model on kagome lattice using symmetric PEPS</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Xiaoyu Dong, Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Frank Verstraete</td></tr>
</tbody></table>

<h3>Context</h3>
<p>The study of topological phases of states is one of the cutting edges of condensed matter physics nowadays. Spin liquid, in which no magnetic ordering appears even at zero temperature, provides a great playground for the study of topological phases of matter. The antiferromagnetic spin-1/2 Heisenberg model on a kagome lattice is one of the simplest models that is predicted to host a spin liquid ground state. Furthermore, there are some real material systems, such as Herbertsmithite, have&nbsp;interactions that are described by this model, which makes the study of this model important. However, due to the complexity of the numerical simulations, the true nature of the spin liquid, whether it is a gapped Z2 spin liquid or a gapless U(1) Dirac spin liquid, is still under debate. In this project, we will use PEPS as the ansatz to find the&nbsp;ground state numerically, and reducing the number of variational parameters by introducing symmetries into it.&nbsp;</p>

<h3>Goal</h3>
<p>Understand how to construct PEPS with Z2 topological order and both onsite and spatial symmetries. Do the numerical simulations to find the ground state and study various physical properties of this state.</p>

<hr><h2>Solving pentagon equations: going to the heart of topological order in exotic materials</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Robijn Vanhove</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Around the 1980's, a whole new class of exotic materials were discovered. These materials exhibit what is known as "topological order": an umbrella term for the many exotic properties these systems can show. One interesting instance of such materials are topological insulators: materials with&nbsp;bulk insulation&nbsp;where&nbsp;a current is allowed to run along the surface.&nbsp;Since then, it has become clear that these new materials are promissing in realizing real and efficient quantum computers and developping quantum error correcting codes, crucial for an efficient implementation of new codes using quantum computers. The theoretical backbone for topological order is what is known as category theory. Although&nbsp;highly mathematical, at the heart of the theoretical description of category theory, relevant for practical implementations of topologically ordered system, is the "Pentagon equation": a system of exponentially growing, coupled non-linear equations. Solving these equations is known as an incredibly hard problem and only analytic solutions are known for systems with a small number of excitation modes (anyons).&nbsp;</p>

<h3>Goal</h3>
<p>The aim of the thesis project is to write performant&nbsp;code for solving these equations, especially for systems with a large number of anyons (number of particles in the system). The aim however is not only on the numerics side, pushing the code as far as possible, since a thourough understaning of the underlying system is needed to make progress. The proposal therefore requiers also some theoretical understanding of topological order and the tensor network methods developed in the group describing such systems.&nbsp;The group already disposes of working code which will be used as a solid base. The student can start by understanding the known methods such as "Smith normal forms" and "Groebner bases" and a&nbsp;highly interesting prospect in making strides is to use the new GPUs available in the group to further push the capabilities of the code. The student will enevitably work on a hard problem that will lead to new results relevant for research in a broad physics and numerics community.&nbsp;</p>

<hr><h2>Tensor network methods for higher dimensional lattice gauge theories</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Lander Burgelman, Laurens Lootens</td></tr>
</tbody></table>

<h3>Context</h3>
<p>The concept of gauge symmetries is ubiquitous in many-body physics. Most notably, it underpins the Standard Model of elementary particle physics where the fundamental interactions of nature arise from the gauging of global symmetries, but gauge theories also appear in the context of low-temperature condensed matter systems. For small coupling regimes, they can be studied using perturbation theory, giving rise to the well-known Feynman diagrammatic approach to quantum field theories. In the theory of quantum electrodynamics, this approach has led to results with an unrivaled precision. In contrast, this perturbative approach breaks down entirely when interactions become strong. Most notably, this is the case for the theory of quantum chromodynamics (QCD) which describes the strong interaction, where all low energy features are essentially non-perturbative.</p>

<p>Currently, the most accurate description of the strongly coupled behavior of gauge theories stems from a discrete formulation in terms of lattice gauge theory [1]. Over the past decades lattice QCD computations based on Monte Carlo sampling have reached impressive accuracy, for instance in the ab initio determination of the light hadron masses. In spite of these remarkable results, lattice Monte Carlo sampling suffers from some significant drawbacks. Firstly, the use of Euclidean time in these calculations does not allow for real-time simulations of dynamical non-equilibrium phenomena, such as those of interest for example in early universe cosmology. In addition, the Monte Carlo sign problem prevents the study of systems with finite fermion densities.</p>

<p>Tensor networks form a variational class of wavefunctions that have proven extremely useful for describing low energy physics of strongly correlated quantum many body systems. They constitute a non-perturbative approach to Hamiltonian systems, support finite fermion densities and allow for the simulation of real-time dynamics. In recent years there have been successful applications of this framework to 1+1 dimensional lattice gauge theories from a numerical perspective, while also leading to a deeper understanding of gauge invariance at the level of the quantum state itself. In the past months, this initial progress was pushed to some first applications in higher dimensional models. Our group has recently made significant advances in the development of novel variational tensor network algorithms which could pave the way to more ambitious simulations of lattices gauge theories in higher dimensions. This forms the topic of this master's thesis.</p>

<p>[1] John B. Kogut. An introduction to lattice gauge theory and spin systems. Reviews of Modern Physics, 51(4):659–713, October 1979.</p>

<h3>Goal</h3>
<p>The goal of this thesis project is to gain a deeper understanding of gauge invariance at the level of quantum states, as well as using these insights for simulating lattice gauge theories. This involves several aspects. The first is a theoretical one, and concerns the group's ongoing quest to capture symmetries and their gauging in lattice models by exploring tensor network realizations of higher-form symmetries and dualities. The second is a numerical aspect, in which these insights would be combined with state-of-the-art variational methods developed in the group to tackle the simulation of higher dimensional lattice gauge theories. Finally, there is an additional technological aspect. Just as insights from the use of quantum simulators have recently been adapted to tensor network studies, the concepts and algorithms developed in this thesis would in turn be investigated in a quantum hardware context. This could potentially lead to advances in the simulation of strongly coupled gauge theories with cold atom quantum simulators, which would be an important application of quantum technologies in the near future.</p>

<hr><h2>Tensor networks as toy models for AdS/CFT</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Laurens Lootens, Marco Deweirdt</td></tr>
</tbody></table>

<h3>Context</h3>
<p>For some time now, one of the most active research topics in high-energy physics has been the study of holographic dualities between quantum gravity in D+1 dimensions and D-dimensional conformal field theory on the boundary. One version of this duality going under the name of the AdS/CFT correspondence has enjoyed the most success, and the correspondence between 3-dimensional gravity in anti-de Sitter and 2-dimensional conformal field theory is particularly tractable due to the exact solvability of 2D CFT. In more recent years, it has been established that such holographic dualities can also be understood from a quantum information theory perspective. Tensor networks have emerged as an especially powerful language for expressing quantum information concepts, and they were used to construct toy models for the AdS3/CFT2 correspondence as error-correcting codes on a hyperbolic geometry, the first of these being named the "HaPPY code" after the authors.</p>

<p><img alt="" src="{{ site.url }}{{ site.baseurl }}/images/thesis/hyperinvariant.png" style="height:368px; width:364px"></p>

<p>At same time, much recent progress has been made in our group in the understanding of critical lattice models described by 2-dimensional conformal field theories using tensor networks. The crucial insight is that these can be obtained from a holographic construction starting from a topological field theory and going down to a conformal field theory. A key feature is the presence of non-local symmetries called topological defects, which govern many of the interesting properties of these conformal field theories, and which admit a beautiful explicit tensor network representation under the form of matrix product operators.</p>

<h3>Goal</h3>
<p>The goal of this thesis is to use the tensor network expertise developed by our group of 2-dimensional conformal field theories to study tensor network models of the AdS3/CFT2 correspondence. Many aspects here are not yet understood, but the tools are there and the time is ripe to make these connections. There is a nonzero overlap with work done in the community of loop quantum gravity, and many of our results have some interpretation in that framework. Recently, researchers working in this community have started to be able to compute observables in the higher dimensional AdS4/CFT3 correspondence as well, using tensor networks as an efficient scheme for calculating such quantities.</p>

<p>The student is expected to familiarize themselves with the state of the art both in tensor network models of AdS/CFT, as well as the holographic construction of critical lattice models from a topogically ordered state. This requires a working knowledge of the theory of tensor networks, conformal field theory, some category theory and various aspects of the AdS/CFT correspondence. The advantage of formulating these problems in terms of tensor networks is that they can be verified numerically using the powerful tensor network toolbox, many aspects of which have been pioneered by our group.</p>

<hr><h2>Tensor networks for relativistic quantum field theory</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Bastiaan Aelbrecht, Benoît Tuybens, Gertian Roose</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Quantum field theory (QFT) provides us with an efficient toolbox for describing high energy physics (elementary particles) as well as low energy physics (condensed matter). In fact, it is one of the big triumphs in physics with showpieces as the standard<img alt="" src="{{ site.url }}{{ site.baseurl }}/images/thesis/fd.png" style="float:right; height:220px; width:420px">&nbsp;model and an accurate description of various exotic states of matter, such as superfluidity and superconductivity. However, QFT is not an easy theory as there are an infinite number of degrees of freedom to consider. The only QFTs that we can solve exactly are non-interacting systems and a handful of special models where there are infinitely many conservation laws. The more realistic (and thus more interesting) aspects demand that we take interactions into account. For certain weakly interacting theories where the coupling constant decreases with the energy scale (as in e.g. quantum electrodynamics) we get away with perturbation theory, elegantly summarised by Feynman diagrams. On the other hand for theories that exhibit asymptotic freedom (such as the strong nuclear force), the coupling gets bigger at low energy scales, and therefore perturbation theory is out of the question.</p>

<p>And yet it are exactly these strongly correlated quantum systems in which we specialize here in Ghent. For such systems, we must focus on the variational principle, which can be briefly summarized as: "Make an educated guess (the ansatz) about the ground state of&nbsp; the system, and&nbsp; minimize the expectation value of the hamiltonian in this state."&nbsp;</p>

<p>Richard Feynman argued about thirty years ago on a conference in Germany, named Variational calculations in quantum field theory, that such a principle would not work for continuous quantum systems. [1] He simply couldn't imagine that an efficient ansatz could be found that (1) was anything else than Gaussian and (2) wherefore expectation values could actually be calculated. However, thanks to insights from quantum information theory in the last decade, we are now able to study (one-dimensional) quantum fields directly in the continuum limit with the variational method.<img alt="" src="{{ site.url }}{{ site.baseurl }}/images/thesis/mpstocmps.png" style="float:right; height:237px; width:320px"></p>

<p>The ansatz under consideration is the continuous Matrix Product State (cMPS), a direct generalization of the enormously successful MPS, heavily used for strongly correlated spin chains. [2] In the past eleven years, this cMPS has been successfully applied to some continuous condensed matter hamiltonians, and hard work has been done on extensions to other boundary conditions and non-translation invariant systems. Even relativistic theories have been studied, but with the caveat that the Lorentz symmetry must be broken softly, because the variational principle will try to optimize all momentum modes at once, hence the UV physics is by far overrepresented and the relevant IR physics is swept under the carpet. [3] In practice this meant adding a UV cut-off in the form of a counterterm in the hamiltonian. Very recently though, a paper has been published on arXiv that suggests a minor adaptation to the cMPS ansatz, in order to optimize relativistic QFT directly without the need to add such a term in the Hamiltonian. [4]</p>

<h3>Goal</h3>
<p>This thesis subject has a theoretical as well as a numerical component. The numerical aspect would be done in the programming language Julia, in which our group already constructed a framework for MPS. The ansatz of Tilloy is new, so there is a lot that can be investigated. As a first acquintance with the subject the results of Tilloy for the real scalar field with quartic self-interaction&nbsp;in 1+1 dimensions, familiar from the course Quantum field theory, should be reproduced. This includes the calculations of the expectation values within the ansatz as well as the actual numerical optimization. What is particularly interesting, is how the error scales as a function of the bond dimension,i.e.&nbsp; the 'size' of the ansatz.&nbsp;</p>

<p>As an expansion, the thesis would apply the developed framework to study the sine-Gordon model. This field theory plays a crucial role in the description of superconduction and also describes the Berezinskii-Kosterlitz-Thouless phase transition that won the 2016 nobel prize for physics.</p>

<p>The objective of this thesis is quite broad, such that the student has sufficient space to steer the project in his preferred direction, acccording to his/her interest and progress in the academic year.&nbsp;<br>
<br>
[1] Lutz Polley and David EL Pottinger. Variational Calculations In Quantum Field Theory:Proceedings Of The International Workshop. World Scientific, 1988.<br>
[2] Frank Verstraete and J Ignacio Cirac. Continuous matrix product states for quantum fields.&nbsp;Physical review letters, 104(19):190405, 2010.<br>
[3] Jutho Haegeman, J Ignacio Cirac, Tobias J Osborne, Henri Verschelde, and Frank Ver-straete. Applying the variational principle to (1+ 1)-dimensional quantum field theories.&nbsp;Physical review letters, 105(25):251601, 2010<br>
[4] Antoine Tilloy. Relativistic continuous matrix product states for quantum fields without cutoff. https://arxiv.org/abs/2102.07741, 2021.</p>

<hr><h2>The symphony between music and quantum mechanics</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Tom Vieijra, Benoît Tuybens</td></tr>
</tbody></table>

<h3>Context</h3>
<p>In the last 20 years, Matrix Product States (MPS) have emerged as one of the most important and accurate models for describing one-dimensional quantum mechanical many-particle systems. Driven by this success, similar problems are attempted to be solved by this description both in and outside of physics. One of these new applications is the use of MPS for tasks within the context of machine learning, such as classifying handwritten numbers or short sound fragments, and time evolution of cellular automata. In this thesis we will apply MPS to music. Machine learning for musical compositions is important, if one thinks about automating finding the genre of a piece of music and recommending new pieces of music to a specific user profile.</p>

<h3>Goal</h3>
<p>Using a data-set consisting of a large number of tracks, we will use MPS to model time-dependent correlations such as the pitch or timbre of the track and extract information such as genre, artist gender or tempo. At a later stage we can look at the effect of coarse graining (renormalization) on the time series, with the aim of efficiently describing longer pieces of music. Another extension is the use of Matrix Product Operators (MPO) to convert two time series describing the same piece of music. This thesis is suitable for students who would like to investigate the relationship between physical methods and non-physical applications. The thesis has a literature review component in which, on the one hand, the methods used within the study of tensor networks are examined and, on the other hand, recent applications of tensor networks within machine learning are examined. In addition, the thesis has an important computational component, where the investigated methods are applied to musical pieces.</p>

<hr><h2>Topological quantum computing through defects and beyond using tensor networks</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Marco Deweirdt, Laurens Lootens, Lander Burgelman</td></tr>
</tbody></table>

<h3>Context</h3>
<p>Topological quantum computing, introduced in 1997 by Kitaev, provides a new and elegant way to protect quantum information against errors by exploiting the inherent robustness of systems with so-called textit{topological order}. In the subsequent 20 years this topic has become a well studied and vast research subject and a plethora of models and tools have been discovered to manipulate these systems, such that they can be used as proper building blocks to construct quantum error correction. Among these developments are the treatment of the boundaries&nbsp;of these systems and their&nbsp;defects, providing new features which in turn enrich the original system. More or less around the same time, Steven White introduced the DMRG algorithm in 1994, which marked the birth of so-called tensor networks. Examples of such networks are the Matrix Product State&nbsp;(MPS) and the Projected Entangled Pair State&nbsp;(PEPS), which target that part of the enormous Hilbert space in which most of the relevant physics takes place. The fact that we can target that corner so precisely is the main reason why we can simulate one-dimensional and two-dimensional systems so successfully today and why&nbsp;we are able to characterize such topological systems through the language of tensor networks. This thesis subject investigates the interface between these two scientific developments and will provide useful and efficient tools to tackle the physics at hand.</p>

<h3>Goal</h3>
<p>The main goal of this thesis is&nbsp;to construct so-called quantum logic&nbsp;gates, e.g.&nbsp;CNOT-gate etc..., using Matrix Product Operators (MPOs), which let&nbsp;us describe topologically ordered systems through strings of matrices and which in turn allow&nbsp;us to characterize all boundaries and defects through the excitations present in the system. Using these tensor network techniques we will investigate how to realize such quantum gates in systems with topological order by&nbsp;procedures known as&nbsp;code deformation&nbsp;and&nbsp;lattice surgery.&nbsp;In such procedures we basically&nbsp;glue together different boundaries on the lattice, resulting in richer and more powerful models to construct quantum computers and quantum memories.</p>

<hr><h2>Topological wormholes in tensor networks</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete</td></tr><tr><td>Begeleider(s):</td><td>Marco Deweirdt, Laurens Lootens</td></tr>
</tbody></table>

<h3>Context</h3>
<p>More then 50 years after the enormous succes of quantum field theories to systematically describe the interactions of particles through the strong, weak and electromagnetic forces, a theory that includes gravity at quantum scales is still one of the most notorious open questions in physics. Besides traditional attempts like string theory and loop quantum gravity, more recent approaches try to explain gravity through the theory of quantum information. The main idea being to quantify gravity through the degree of entanglement shared by two particles. This lead to the famous ER = EPR conjecture by Susskind in 2016, identifying entanglement or&nbsp;spooky action at a distance&nbsp;(EPR) with so-called&nbsp;Einstein-Rosen bridges&nbsp;or&nbsp;wormholes&nbsp;(ER) or in more abstract terms, the geometry of spacetime, and thus with gravity in the setting of general relativity.</p>

<p><img alt="Picture from Wikipedia" src="{{ site.url }}{{ site.baseurl }}/images/thesis/Wormhole-demo.png" style="height:480px; width:640px"></p>

<p>Picture from Wikipedia</p>

<p>The study of quantum information is also driven by the search for quantum computing algorithms, which&nbsp;exploit&nbsp;the quantum nature of qubits or spins to complete tasks, deemed insurmountable for classical computers.&nbsp;Topological quantum computation&nbsp;(Kitaev, 1997), is one of the most promising methods&nbsp;amongst them&nbsp;and makes use of&nbsp;the inherent robustness of systems with topological order to protect quantum computers from errors. Recent developments suggest that we can realize wormholes in such topologically ordered systems by punching some holes in them and entangling the defects created in the process, estabilishing ER = EPR on the lattice.</p>

<p>The tools available to us are so-called&nbsp;tensor network states, such as&nbsp;Matrix Product States&nbsp;(MPS) and&nbsp;Projected Entangled Pair States&nbsp;(PEPS), which specifically target the physically relevant corner of the immense Hilbert space, providing an efficient description in terms of the information necessary to characterize the system at hand, resulting in the great succes of describing one- and two-dimensional systems using tensor networks. This thesis subject finds itself at the crossroads of the discplines mentioned above.</p>


<h3>Goal</h3>
<p>The goal of this thesis is to find out how to create entangled defects&nbsp;in the language of tensor networks, estabilishing an effective wormhole in the lattice and to study its behavior in terms of the topological excitations&nbsp;emerging from the system. The student will use a&nbsp;formalism based on&nbsp;Matrix Product Operators&nbsp;(MPOs)&nbsp;to characterize topologically ordered systems and describe the associated boundaries and defects present in such systems. Having obtained an adequate understanding of this formalism, the student will apply this system to the so-called toric code, introduced by Kitaev, and will try to replicate entangled defects in this system. Further study then includes an investigation of the features of quantum codes with this new kind of defects or wormholes and a generalization to more complicated models.</p>

<hr><h2>Tropical Tensor Networks</h2>
<table border="0">
<tbody><tr><td>Promotor(en):</td><td>Frank Verstraete, Jutho Haegeman</td></tr><tr><td>Begeleider(s):</td><td>Lukas Devos</td></tr>
</tbody></table>

<h3>Context</h3>
<p>For a statistical mechanics system on a lattice, computing the partition function leads to the knowledge of all physical properties (magnetisation, pressure, specific heat, ...) and for a local Hamiltonian this is done by summing over all possible configurations of the system, where each configuration is weighted with the product of the local Boltzmann weights. Conveniently, this can be translated to the language of tensor networks by assigning a tensor to each vertex and contracting the resulting diagram.</p>

<p>Once in the language of tensor networks, there exists a plethora of tools and algorithms, readily implemented on a computer, for the exact and/or approximate contraction of the resulting network. Nevertheless, in the zero temperature limit, dealing with exponentially large or small numbers on computers with finite precision numerics leads to issues. This problem can be resolved by working with the exponents directly and going to the zero-temperature limit, such that new addition and multiplication laws naturally appear, by replacing addition with a max operation, and replacing multiplication with regular addition.</p>

<p>These are the defining relations of the tropical semiring [1], or the max-plus algebra. Working with tensors over this semiring instead of over the usual complex numbers circumvents the aforementioned problems, while still retaining the commutative, associative an distributive properties, but at the cost of losing the possibility to define an additive inverse.</p>

<p>[1] Wikipedia. Tropical semiring — Wikipedia, the free encyclopedia. <a href="https://en.wikipedia.org/wiki/Tropical_semiring">https://en.wikipedia.org/wiki/Tropical_semiring</a>, 2021.</p>


<h3>Goal</h3>
<p>The student would commence by gaining an understanding of tropical numbers and their implementation, using the results of [2] as a starting point. Combining this with existing state-of-the-art tensor network methods of our group, the goal is to explore what stands and what breaks down by making the switch to tropical numbers. Ultimately, the goal is to simulate classical systems in their low temperature regime, comparing the accuracy and performance of these new methods with analytic results, as well as with standard tensor network methods.</p>

<p>Finally, the tropical numbers lend themselves not only to the simulation of classical systems at low temperatures, but are also important in the context of combinatorical problems such as frustrated spin glass systems [2], in system- and control theory [3], or for deep neural networks [4].</p>

<p>[2] Liu, J.-G., Wang, L., Zhang, P., 2021. Tropical Tensor Network for Ground States of Spin Glasses. arXiv:2008.06888.</p>

<p>[3] Quadrat, J.-P., 1995. Max-Plus Algebra and Applications to System Theory and Optimal Control, in: Chatterji, S.D. (Ed.), Proceedings of the International Congress of Mathematicians. Birkhäuser Basel, Basel, pp. 1511–1522. <a href="https://doi.org/10.1007/978-3-0348-9078-6_148">https://doi.org/10.1007/978-3-0348-9078-6_148</a></p>

<p>[4] Zhang, L., Naitzat, G., Lim, L.-H., 2018. Tropical Geometry of Deep Neural Networks. arXiv:1805.07091.</p>