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
doi: https://journals.aps.org/pra/abstract/10.1103/4ds8-1jt8
type: journal
figure: /images/papers/free-energy.png
feature-title: Constrained Free Energy Minimization
feature-description: Using free-energy minimization to design thermal states and stabilizer thermodynamic systems
image: /images/papers/free-energy.png
featured: true
feature-order: 13
bibtex: |-

    @article{4ds8-1jt8,
      title = {Constrained free energy minimization for the design of thermal states and stabilizer thermodynamic systems},
      author = {Minervini, Michele and Chin, Madison and Kupperman, Jacob and Liu, Nana and Luo, Ivy and Ly, Meghan and Rethinasamy, Soorya and Wang, Kathie and Wilde, Mark M.},
      journal = {Phys. Rev. A},
      volume = {113},
      issue = {4},
      pages = {042407},
      numpages = {32},
      year = {2026},
      month = {Apr},
      publisher = {American Physical Society},
      doi = {10.1103/4ds8-1jt8},
      url = {https://link.aps.org/doi/10.1103/4ds8-1jt8}
    }


---

A quantum thermodynamic system is described by a Hamiltonian and a list of conserved, noncommuting charges, and a fundamental goal is to determine the minimum energy of the system subject to constraints on the charges. Recently, Liu et al. [arXiv:2505.04514] proposed first- and second-order classical and hybrid quantum-classical algorithms for solving a dual chemical potential maximization problem, and they proved that these algorithms converge to global optima by means of gradient-ascent approaches. In this paper, we benchmark these algorithms on several problems of interest in thermodynamics, including one- and two-dimensional quantum Heisenberg models with nearest- and next-nearest-neighbor interactions and with the charges set to the total 𝑥, 𝑦, and 𝑧 magnetizations. We also offer an alternative compelling interpretation of these algorithms as methods for designing ground and thermal states of controllable Hamiltonians, with potential applications in molecular and material design. Furthermore, we introduce stabilizer thermodynamic systems as thermodynamic systems based on stabilizer codes, with the Hamiltonian constructed from a given code's stabilizer operators and the charges constructed from the code's logical operators. We benchmark the aforementioned algorithms on several examples of stabilizer thermodynamic systems, including those constructed from the one-to-three-qubit repetition code, the perfect one-to-five-qubit code, and the two-to-four-qubit error-detecting code. Finally, we observe that the aforementioned hybrid quantum-classical algorithms, when applied to stabilizer thermodynamic systems, can serve as alternative methods for encoding quantum information into stabilizer codes at a fixed temperature, and we provide an effective method for warm-starting these encoding algorithms whenever a single qubit is encoded into multiple physical qubits.