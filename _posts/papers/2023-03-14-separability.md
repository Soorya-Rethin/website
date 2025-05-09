---
layout: paper
categories: papers
permalink: papers/separability
id: separability
title: "Schrödinger as a Quantum Programmer: Estimating Entanglement via Steering"
authors: 
  - Aby Philip
  - Soorya Rethinasamy
  - Vincent Russo
  - Mark M. Wilde
venue: Quantum Journal
year: 2023
url: /papers/separability
pdf: https://arxiv.org/abs/2303.07911
doi: 10.22331/q-2024-06-11-1366
type: journal
figure: /images/papers/separability.png
feature-title: "Schrödinger as a Quantum Programmer"
feature-description: Quantum algorithm to estimating Entanglement via Steering
image: /images/featured/separability.png
featured: true
feature-order: 5
bibtex: |-

    @article{Philip2024schrodingeras,
        doi = {10.22331/q-2024-06-11-1366},
        url = {https://doi.org/10.22331/q-2024-06-11-1366},
        title = {Schr{\"{o}}dinger as a {Q}uantum {P}rogrammer: {E}stimating {E}ntanglement via {S}teering},
        author = {Philip, Aby and Rethinasamy, Soorya and Russo, Vincent and Wilde, Mark M.},
        journal = {{Quantum}},
        issn = {2521-327X},
        publisher = {{Verein zur F{\"{o}}rderung des Open Access Publizierens in den Quantenwissenschaften}},
        volume = {8},
        pages = {1366},
        month = jun,
        year = {2024}
    }

---

Quantifying entanglement is an important task by which the resourcefulness of a quantum state can be measured. Here, we develop a quantum algorithm that tests for and quantifies the separability of a general bipartite state by using the quantum steering effect, the latter initially discovered by Schrödinger. Our separability test consists of a distributed quantum computation involving two parties: a computationally limited client, who prepares a purification of the state of interest, and a computationally unbounded server, who tries to steer the reduced systems to a probabilistic ensemble of pure product states. To design a practical algorithm, we replace the role of the server with a combination of parameterized unitary circuits and classical optimization techniques to perform the necessary computation. The result is a variational quantum steering algorithm (VQSA), a modified separability test that is implementable on quantum computers that are available today. We then simulate our VQSA on noisy quantum simulators and find favorable convergence properties on the examples tested. We also develop semidefinite programs, executable on classical computers, that benchmark the results obtained from our VQSA. Thus, our findings provide a meaningful connection between steering, entanglement, quantum algorithms, and quantum computational complexity theory. They also demonstrate the value of a parameterized mid-circuit measurement in a VQSA.