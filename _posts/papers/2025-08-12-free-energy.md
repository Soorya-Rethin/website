---
layout: paper
categories: papers
permalink: papers/free-energy
id: free-energy
title: "Constrained free energy minimization for the design of thermal states and stabilizer thermodynamic systems"
authors: 
  - Michele Minervini
  - Madison Chin
  - Jacob Kupperman
  - Nana Liu
  - Ivy Luo
  - Meghan Ly
  - Soorya Rethinasamy
  - Kathie Wang
  - Mark M. Wilde
venue: arXiv
year: 2025
url: /papers/free-energy
pdf: https://arxiv.org/abs/2508.09103
doi: https://doi.org/10.48550/arXiv.2508.09103
type: preprint
figure: /images/papers/free-energy.png
feature-title: Constrained Free Energy Minimization
feature-description: Using free-energy minimization to design thermal states and stabilizer thermodynamic systems
image: /images/papers/free-energy.png
featured: true
feature-order: 13
bibtex: |-

    @misc{rethinasamy2024neutronnucleusdynamicssimulationsquantum,
      title={Neutron-nucleus dynamics simulations for quantum computers}, 
      author={Soorya Rethinasamy and Ethan Guo and Alexander Wei and Mark M. Wilde and Kristina D. Launey},
      year={2024},
      eprint={2402.14680},
      archivePrefix={arXiv},
      primaryClass={quant-ph},
      url={https://arxiv.org/abs/2402.14680}, 
    }

---

With a view toward addressing the explosive growth in the computational demands of nuclear structure and reactions modeling, we develop a novel quantum algorithm for neutron-nucleus simulations with general potentials, which provides acceptable bound-state energies even in the presence of noise, through the noise-resilient training method. In particular, the algorithm can now solve for any band-diagonal to full Hamiltonian matrices, as needed to accommodate a general central potential. This includes exponential Gaussian-like potentials and ab initio inter-cluster potentials (optical potentials). The approach can also accommodate the complete form of the chiral effective-field-theory nucleon-nucleon potentials used in ab initio nuclear calculations. We make this potential available for three different qubit encodings, including the one-hot (OHE), binary (BE), and Gray encodings (GE), and we provide a comprehensive analysis of the number of Pauli terms and commuting sets involved. We find that the GE allows for an efficient scaling of the model-space size \\( N\\) (or number of basis states used) and is more resource efficient not only for tridiagonal Hamiltonians, but also for band-diagonal Hamiltonians having bandwidth up to \\( N\\). We introduce a new commutativity scheme called distance-grouped commutativity (DGC) and compare its performance with the well-known qubit-commutativity (QC) scheme. We lay out the explicit grouping of Pauli strings and the diagonalizing unitary under the DGC scheme, and we find that it outperforms the QC scheme, at the cost of a more complex diagonalizing unitary. Lastly, we provide first solutions of the neutron-alpha dynamics from quantum simulations suitable for NISQ processors, using an optical potential rooted in first principles, and a study of the bound-state physics in neutron-Carbon systems, along with a comparison of the efficacy of the OHE and GE.