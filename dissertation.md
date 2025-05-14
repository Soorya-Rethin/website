---
layout: page
title: "Distinguishability, Symmetry, and Energy Estimation: Quantum Algorithms and Complexity"
permalink: dissertation/
redirect_from: defense/
jsarr:
- js/scripts.js
---

<span class="dissertation-subtitle">
This dissertation is a collection of quantum algorithms designed to estimate different quantities. These quantities belong to three different domains: distinguishability, symmetry, and energy. The algorithms are all based on the *variational principle* -- using a parameterized state to guess the solution and training for the optimal parameters. The work also analyses the quantum computational complexity of the various estimation problems, connecting the complexity heirarchy and the different estimation problems.
<span>

We now go into detail of the various algorithms in the three different domains.

##### 1. Distinguishability

Distinguishability measures form the basis of all information processing tasks. The ability to distinguish between different outcomes is fundamental. In this chapter, we put forth several quantum algorithms to estimate various state and channel distinguishability measures, like the fidelity, trace distance, diamond distance, among others. The results of this section are based on the paper <a href="{{ site.url }}/papers/distinguish" class="sc">Distinguish</a>.

##### 2. Symmetry

Symmetry plays a fundamental rule in physics and quantum information science. It dictates allowed transitions, resourceful states, and can be used to simplify the understanding complex systems. In this work, we put forth four notions of symmetry and show results for a wide range of groups. We also provide operation interpretations for quantities known as *maximum symmetric fidelities* in terms of the proposed quantum algorithms. Lastly, we also connect the symmetry-testing problems to the quantum computational complexity heirarchy. The results of this section are based on the papers <a href="{{ site.url }}/papers/test-symmetry" class="sc">Testing Symmetry</a> and <a href="{{ site.url }}/papers/complex-symmetry" class="sc">Symmetry Complexity</a>.

##### 3. Energy

The atomic nucleus is a quantum many-body system made of nucleons that are subject to residual strong forces that have no analytical solution. For an A-particle system, the nuclear problem needs to be solved numerically in the infinite- dimensional Hilbert space of A particles with Hamiltonians that admit state-of-the-art nucleon-nucleon (NN) forces, often three-nucleon (3N), and even four-nucleon (4N) forces. This leads to the so-called scale explosion problem in nuclear structure calculations, i.e., the explosive growth in computational resource demands with increasing number of particles and size of the spaces in which they reside. In this paper, we provide a generalized, extensible, and strong mathemati- cal formulation of three mappings to qubits: one-hot, binary, and Gray encodings, explore their relative advantages, and illustrate these for simulations with the above-mentioned potentials. The results of this section are based on the paper <a href="{{ site.url }}/papers/nuclear" class="sc">Nuclear Quantum Computing</a>.

***

<div class="l-middle">
    {% include dissertation/document.html details=true location=page %}
</div>

## Thesis Defense

**Soorya Rethinasamy**  
Applied and Engineering Physics      
Cornell University

**Date:** Monday, May 28, 2025   
**Time:** 8:00am - 9:30am EST  
**Location:** Rhodes Hall   

**Committee**  
Mark M. Wilde - *Advisor, Cornell University*  
Karan Mehta - *Committee Member, Cornell University*  
Valla Fatemi - *Committee Member, Cornell University*  

{% for talk in site.data.dissertation.talks %}
{% if talk.key == "defense" %}
{% include dissertation/talk.html talk=talk %}
{% endif %}
{% endfor %}

<!-- **Materials**   -->
* [Slides][talk-high-db]

**Bio (from May 2025)**  
Soorya Rethinasamy is a fifth-year graduate student in the Applied and Engineering Physics Department at Cornell University. He received his Bachelor of Engineering (Hons.) in Computer Science and his Master of Science (Hons.) in Physics from the Birla Institute of Technology and Science, Pilani. He began his Ph.D. at Louisiana State University in 2021 and transferred to Cornell University in 2022.

During his tenure, he has authored several publications and presented his work at multiple conferences. He has also mentored several high school and undergraduate students in quantum computing, resulting in collaborative research publications. His research field is the design and analysis of quantum algorithms. He attended the IBM Summer School on quantum error correction and interned at the Global Technology Applied Research Team at JP Morgan Chase.

[talk-low]: {{ site.url }}/talk-low-quality.pdf
[talk-high]: {{ site.url }}/talk-high-quality.pdf
[talk-export]: https://youtu.be/k8fzkxxxyr8
[talk-low-db]: https://www.dropbox.com/s/b4aqsp6ota3zani/defense-low-quality.pdf?dl=0
[talk-high-db]: https://drive.google.com/file/d/1AtlI46LJprmIfG6rpV6iao_qYlMlub3A/view?usp=sharing
[cv]: https://fredhohman.com/cv
[cv-pdf]: https://fredhohman.com/cv.pdf
[statement]: {{ site.url }}/research-statement.pdf

[gamut]: {{ site.url }}/papers/gamut
[telegam]: {{ site.url }}/papers/telegam
[deepvis]: {{ site.url }}/papers/deepvis
[summit]: {{ site.url }}/papers/summit
[parametric]: {{ site.url }}/papers/parametric
[interactive-articles]: {{ site.url }}/papers/interactive-articles