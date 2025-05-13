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

<!--User research with practitioners guides the creation of our novel operationalization for interpretability, which helps tool builders design interactive systems for model and prediction explanations. We develop two such visualization systems, <a href="{{ site.url }}/papers/gamut" class="sc">Gamut</a> and <a href="{{ site.url }}/papers/telegam" class="sc">TeleGam</a>, which we deploy at Microsoft Research as a design probe to investigate the emerging practice of interpreting models. -->

##### 2. Symmetry

<!--Our first-of-its-kind <a href="{{ site.url }}/papers/deepvis" class="sc">Interrogative Survey</a> reveals critical yet understudied areas of deep learning interpretability research, such as the lack of higher-level explanations for neural networks. Through <a href="{{ site.url }}/papers/summit" class="sc">Summit</a>, an interactive visualization system, we present the first scalable graph representation that summarizes and visualizes what features deep learning models learn and how those features interact to make predictions (e.g., InceptionNet trained on ImageNet with 1.2M+ images).-->

##### 3. Energy

<!--We use <a href="{{ site.url }}/papers/interactive-articles" class="sc">Interactive Articles</a>, a new medium on the web, to teach people about machine learning's capabilities and limitations, while developing a new interactive publishing initiative called the <a href="{{ site.url }}/papers/parametric" class="sc">Parametric Press</a>. From our success publishing interactive content at scale, we generalize and detail the affordances of interactive articles by connecting techniques used in practice and the theories and empirical evaluations put forth by diverse disciplines of research.
-->

***

This thesis contributes to *information visualization*, *machine learning*, and more importantly *their intersection*, including open-source interactive interfaces, scalable algorithms, and new, accessible communication paradigms. Our work is making significant impact in industry and society: our visualizations have been deployed and demoed at Microsoft and built into widely-used interpretability toolkits, our interactive articles have been read by 250,000+ people, and our interpretability research is supported by NASA.

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