---
layout: paper
categories: papers
permalink: papers/rotational
id: rotational
title: "Efficacious qubit mappings for quantum simulations of the \\(^{12}C\\) rotational band"
authors:
  - Darin C. Mumma
  - Zhonghao Sun
  - Alexis Mercenne
  - Kristina D. Launey
  - Soorya Rethinasamy
  - James A. Sauls
venue: 2024 IEEE Computer Society Annual Symposium on VLSI
venue-shorthand: ISVLSI
year: 2024
url: /papers/rotational
pdf: https://arxiv.org/abs/2412.06979
doi: 10.1109/ISVLSI61997.2024.00119
type: conference
figure: /images/papers/rotational.png
feature-title: "Quantum Simulations of the \\(^{12}C\\) Rotational Band"
feature-description: "Exploring the low lying strcture of the \\(^{12}C\\) nucleus."
image: /images/featured/rotational.png
featured: true
feature-order: 12
bibtex: |-

    @INPROCEEDINGS{10682675,
        author={Mumma, Darin C. and Sun, Zhonghao and Mercenne, Alexis and Launey, Kristina D. and Rethinasamy, Soorya and Sauls, James A.},
        booktitle={2024 IEEE Computer Society Annual Symposium on VLSI (ISVLSI)}, 
        title={Efficacious Qubit Mappings for Quantum Simulations of the 12C Rotational Band}, 
        year={2024},
        volume={},
        number={},
        pages={627-631},
        keywords={Performance evaluation;Qubit;Noise;Very large scale integration;Encoding;Stability analysis;Reliability;Quantum computing;noise;encoding;Gray encoding;nuclear structure;symmetry -adapted basis},
        doi={10.1109/ISVLSI61997.2024.00119}
    }

---

Solving atomic nuclei from first principles places enormous demands on computational resources, which grow exponentially with increasing number of particles and the size of the space they occupy. We present first quantum simulations based on the variational quantum eigensolver for the low-lying structure of the \\(^{12}C\\) nucleus that provide acceptable bound-state energies even in the presence of noise. We achieve this by taking advantage of two critical developments. First, we utilize an almost perfect symmetry of atomic nuclei that, in a complete symmetry-adapted basis, drastically reduces the size of the model space. Second, we use the efficacious Gray encoding, for which it has been recently shown that it is resource efficient, especially when coupled with a near band -diagonal structure of the nuclear Hamiltonian.