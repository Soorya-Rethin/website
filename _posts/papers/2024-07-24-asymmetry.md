---
layout: paper
categories: papers
permalink: papers/asymmetry
id: asymmetry
title: "Quantum Algorithms for Realizing Symmetric, Asymmetric, and Antisymmetric Projectors"
authors: 
  - Margarite L. LaBorde
  - Soorya Rethinasamy
  - Mark M. Wilde
venue: arXiv
year: 2024
url: /papers/asymmetry
pdf: https://arxiv.org/abs/2407.17563
doi: https://doi.org/10.48550/arXiv.2407.17563
type: preprint
figure: /images/papers/asymmetry.png
feature-title: Symmetric, Asymmetric, and Antisymmetric Projectors
feature-description: Quantum algorithms to realize different projections and their concatenations.
image: /images/featured/asymmetry.png
featured: true
feature-order: 11
bibtex: |-

    @misc{laborde2024quantumalgorithmsrealizingsymmetric,
      title={Quantum Algorithms for Realizing Symmetric, Asymmetric, and Antisymmetric Projectors}, 
      author={Margarite L. LaBorde and Soorya Rethinasamy and Mark M. Wilde},
      year={2024},
      eprint={2407.17563},
      archivePrefix={arXiv},
      primaryClass={quant-ph},
      url={https://arxiv.org/abs/2407.17563}, 
    }

---

In quantum computing, knowing the symmetries a given system or state obeys or disobeys is often useful. For example, Hamiltonian symmetries may limit allowed state transitions or simplify learning parameters in machine learning applications, and certain asymmetric quantum states are known to be resourceful in various applications. Symmetry testing algorithms provide a means to identify and quantify these properties with respect to a representation of a group. In this paper, we present a collection of quantum algorithms that realize projections onto the symmetric subspace, as well as the asymmetric subspace, of quantum systems. We describe how this can be modified to realize an antisymmetric projection as well, and we show how projectors can be combined in a systematic way to effectively measure various projections in a single quantum circuit. Using these constructions, we demonstrate applications such as testing for Werner-state symmetry and estimating Schmidt ranks of bipartite states, supported by experimental data from IBM Quantum systems. This work underscores the pivotal role of symmetry in simplifying quantum calculations and advancing quantum information tasks.