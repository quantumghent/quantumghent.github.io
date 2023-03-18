---
title: "Downfolding the high dimensional space to perform quantum-mechanical simulations for strongly correlated functional materials"
promoter: Veronique Van Speybroeck, Frank Verstraete
supervisor: Laurens Vanderstraeten
contact: Laurens Vanderstraeten
topic: "Correlated Quantum Materials"
year: "2023"
---

#### Context

In principle, the Schrödinger equation allows us to fully predict a system’s multidimensional wavefunction and behavior. However, solving this equation exactly is not trivial and even impossible for realistic materials containing more than a handful degrees of freedom. Density functional theory (DFT), in which the 3D electron density is the central quantity instead of the multidimensional wavefunction, is therefore the most popular quantum mechanical approach in solid state science nowadays. However, the accuracy of a DFT calculation strongly depends on which of the many available exchange-correlation functionals is chosen.[1] Furthermore, the currently available functionals all fail in the case of systems exhibiting strong electron correlation. This typically occurs when electrons become localized, density fluctuations vary widely over the system, and bands crossing the Fermi energy have a narrow bandwidth. This is the case, for instance, in transition metal-compounds, rare-earth compounds, and organic conductors. Strong electron correlation should therefore be taken into account by using many-body perturbation techniques (MBPT), such as GW and the random phase approximation (RPA), or wavefunction based tensor networks (TN). The latter method however come at a higher computational cost, therefore a viable strategy consists in constructing effective Hamiltonians, where higher accuracy calculations are conducted in a lower dimensional space made of the specific electronic bands that are responsible for the strong electron correlations, see Fig. 1.

Three main challenges arise when solving the Schrödinger equation with this hybrid DFT/TN approach. First, constructing the lower dimensional space. Second, creating the effective Hamiltonian for the lower dimensional space. Third, solving the effective Hamiltonian with the TN methodology that accurately takes electron correlation into account.

To solve the first challenge, we perform DFT calculations and isolate the bands that are close to the Fermi level. With the eigenfunctions of those bands we construct maximally localized Wannier functions (MLWFs). Wannier functions are a set of real-space localized orbitals forming the real-space counterpart of Bloch orbitals.[2],[3] Secondly, we construct the effective Hamiltonian by evaluating the one-and two-body terms of the Schrödinger equation for this set of MLWFs. However, complications arise, both the on-site interaction (one-body) and the interaction between the particles in the low-dimensional space (two-body) are affected by the electrons in the downfolded space. To account for this, we can apply GW to incorporate self-energy effects and constrained RPA to incorporate the screening effect of the downfolded electrons. Finally, we solve the effective Hamiltonian by executing the tensor network methodology.

#### Goal

In this thesis, it is our aim to investigate and improve the methodology to construct the effective Hamiltonians. First, more insight should be obtained about which bands to select. At the moment, there are a few heuristics that can be used to select the bands that are responsible for the strong correlation. Namely, partially filled p, d, and f bands with a narrow bandwidth.[4] However, a deeper understanding of the error introduced by neglecting certain bands in the low dimensional space is currently lacking. Moreover, if the bands of the selected and downfolded subspaces cross (i.e. entangled bands) both spaces are no longer necessarily orthogonal and alternative methods to construct the effective Hamiltonian should be explored.[4] Second, the effect of the DFT XC functional should be investigated as the lower dimensional space is constructed from the DFT orbitals. Moreover, we should also address the double counting error. As the one-body on-site interactions are derived from DFT, the exchange and correlation interactions between the electron in the low dimensional space are incorporated both in the one-and two-body terms of the effective Hamiltonian and therefore counted twice. Different methods to correct for this double counting can be explored.[4] To achieve this goal, the student can either use the existing software that has already been employed or create their own implementation, which would provide greater flexibility in constructing effective Hamiltonians.

Two specific systems featuring strong electron correlation will be investigated in this thesis, both shown in Fig. 2. At first instance, you will use the hybrid DFT/TN scheme to determine accurate ground state energies of the metastable phases of flexible metal-organic frameworks such as MIL-53(Fe).[5] DFT fails in this regard, because the presence of various possible spin configurations has a large impact on the electron properties. A second system of interest in this thesis proposal is rare-earth doped metal halide perovskites (MHPs) such as CsPbI3.[6] Compared to DFT, GW drastically improves to prediction of the band gaps. However, rare-earth doping can severely increase the electron correlation and the DFT/TN methodology might be necessary to get accurate band gaps.

This thesis relies on a collaboration between the Center for Molecular Modeling (Van Speybroeck) having ample expertise in the properties of technologically important materials and their simulation with Density Functional Theory Methods and the Quantum Group (Verstraete) having ample expertise in tensor networks and the theory of quantum entanglement and it application to condensed matter systems.  The potential student for this topic should have interest in fundamental aspects of quantum simulations and their application to important materials for engineering applications. 

#### References

[1] N. Mardirossian, M. Head-Gordon, Mol. Phys. 115: 2315, 2017.

[2] N. Marzari, A.A. Mostofi, J.R. Yates, I. Souza, D. Vanderbilt, Rev. Mod. Phys. 84: 1419, 2012.

[3] G.H. Wannier, Phys. Rev. 117: 432, 1960.

[4] M. Imada, T. Miyake, J. Phys. Soc. Japan., 79: 112001, 2010.

[5] F. Millange, N. Guillou, R.I. Walton, J.-M. Grenèche, I. Margiolaki, G. Férey, Chem. Commun. 2008: 4732, 2008.

[6] J.A. Steele, H. Jin, I. Dovgaliuk, R.F. Berger, T. Braeckevelt, H. Yuan, C. Martin, E. Solano, K. Lejaeghere, S.M.J. Rogge, C. Notebaert, W. Vandezande, K.P.F. Janssen, B. Goderis, E. Debroye, Y.-K. Wang, Y. Dong, D. Ma, M. Saidaminov, H. Tan, Z. Lu, V. Dyadkin, D. Chernyshov, V. Van Speybroeck, E.H. Sargent, J. Hofkens, M.B.J. Roeffaers, Science 365: 679, 2019.
