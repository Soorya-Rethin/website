---
layout: paper
categories: papers
permalink: papers/distinguish
id: distinguish
title: "Estimating Distinguishability Measures on Quantum Computers"
authors: 
  - Soorya Rethinasamy
  - Rochisha Agarwal
  - Kunal Sharma
  - Mark M. Wilde
venue: Physical Review A
venue-shorthand: Phys. Rev. A
year: 2021
url: /papers/distinguish
pdf: https://arxiv.org/abs/2108.08406
video: https://www.youtube.com/watch?v=K9EJejcidwU
doi: 10.1103/PhysRevA.108.012409
type: journal
figure: /images/papers/distinguish.pdf
feature-title: Estimating Distinguishability Measures on Quantum Computers
feature-description: Quantum Algorithms to estimate how distinguishable to states/channels are.
image: /images/featured/distinguish.pdf
slides: /slides/distinguish-slides.pdf
poster: /assets/distinguish-poster.pdf
featured: true
feature-order: 4
bibtex: |-

    @article{PhysRevA.108.012409,
        title = {Estimating distinguishability measures on quantum computers},
        author = {Rethinasamy, Soorya and Agarwal, Rochisha and Sharma, Kunal and Wilde, Mark M.},
        journal = {Phys. Rev. A},
        volume = {108},
        issue = {1},
        pages = {012409},
        numpages = {36},
        year = {2023},
        month = {Jul},
        publisher = {American Physical Society},
        doi = {10.1103/PhysRevA.108.012409},
        url = {https://link.aps.org/doi/10.1103/PhysRevA.108.012409}
        }

---

The performance of a quantum information processing protocol is ultimately judged by distinguishability measures that quantify how distinguishable the actual result of the protocol is from the ideal case. The most prominent distinguishability measures are those based on the fidelity and trace distance, due to their physical interpretations. In this paper, we propose and review several algorithms for estimating distinguishability measures based on trace distance and fidelity. The algorithms can be used for distinguishing quantum states, channels, and strategies (the last also known in the literature as "quantum combs"). The fidelity-based algorithms offer novel physical interpretations of these distinguishability measures in terms of the maximum probability with which a single prover (or competing provers) can convince a verifier to accept the outcome of an associated computation. We simulate many of these algorithms by using a variational approach with parameterized quantum circuits. We find that the simulations converge well in both the noiseless and noisy scenarios, for all examples considered. Furthermore, the noisy simulations exhibit a parameter noise resilience. Finally, we establish a strong relationship between various quantum computational complexity classes and distance estimation problems.