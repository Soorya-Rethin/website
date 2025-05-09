---
layout: paper
categories: papers
permalink: papers/test-symmetry
id: test-symmetry
title: "Testing Symmetry on Quantum Computers"
authors: 
  - Margarite L. LaBorde
  - Soorya Rethinasamy
  - Mark M. Wilde
venue: Quantum Journal
year: 2021
url: /papers/test-symmetry
pdf: https://arxiv.org/abs/2105.12758
video: https://www.youtube.com/watch?v=uJZ1dKXy5Ws
doi: 10.22331/q-2023-09-25-1120
type: journal
figure: /images/papers/test-symmetry.png
feature-title: Testing Symmetry on Quantum Computers
feature-description: Quantum Algorithms to test the symmetry of quantum states.
image: /images/featured/test-symmetry.png
slides: /slides/test-symmetry.pdf
featured: true
feature-order: 3
bibtex: |-

    @article{LaBorde2023testingsymmetry,
        doi = {10.22331/q-2023-09-25-1120},
        url = {https://doi.org/10.22331/q-2023-09-25-1120},
        title = {Testing symmetry on quantum computers},
        author = {LaBorde, Margarite L. and Rethinasamy, Soorya and Wilde, Mark M.},
        journal = {{Quantum}},
        issn = {2521-327X},
        publisher = {{Verein zur F{\"{o}}rderung des Open Access Publizierens in den Quantenwissenschaften}},
        volume = {7},
        pages = {1120},
        month = sep,
        year = {2023}
        }
---

Symmetry is a unifying concept in physics. In quantum information and beyond, it is known that quantum states possessing symmetry are not useful for certain information-processing tasks. For example, states that commute with a Hamiltonian realizing a time evolution are not useful for timekeeping during that evolution, and bipartite states that are highly extendible are not strongly entangled and thus not useful for basic tasks like teleportation. Motivated by this perspective, this paper details several quantum algorithms that test the symmetry of quantum states and channels. For the case of testing Bose symmetry of a state, we show that there is a simple and efficient quantum algorithm, while the tests for other kinds of symmetry rely on the aid of a quantum prover. We prove that the acceptance probability of each algorithm is equal to the maximum symmetric fidelity of the state being tested, thus giving a firm operational meaning to these latter resource quantifiers. Special cases of the algorithms test for incoherence or separability of quantum states. We evaluate the performance of these algorithms on choice examples by using the variational approach to quantum algorithms, replacing the quantum prover with a parameterized circuit. We demonstrate this approach for numerous examples using the IBM quantum noiseless and noisy simulators, and we observe that the algorithms perform well in the noiseless case and exhibit noise resilience in the noisy case. We also show that the maximum symmetric fidelities can be calculated by semi-definite programs, which is useful for benchmarking the performance of these algorithms for sufficiently small examples. Finally, we establish various generalizations of the resource theory of asymmetry, with the upshot being that the acceptance probabilities of the algorithms are resource monotones and thus well motivated from the resource-theoretic perspective.