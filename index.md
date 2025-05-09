---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/portrait.jpg"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Soorya Rethinasamy</h1>
			<div id="intro-subtitle">Physics Ph.D. at Cornell University</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
		<a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a>
	</div>
	<div>
		I design and study quantum algorithms. I am pursuing my Ph.D. from Cornell University, working with <a href="https://www.markwilde.com">Dr. Mark M. Wilde</a>. I have worked on several broad areas, including symmetries, distinguishability measures, variational algorithms, among others. 
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title" style="margin-bottom: 1.5rem;">
  <a href="/cv/#publications">Research Publications</a>
</h2>

<div class="l-text">
	<div class="cover-wrapper cover-wrapper-3-col">
		{% assign sortedPublications = site.categories.papers | sort: 'feature-order' | reverse %}
		{% for feature in sortedPublications %}
			{% if feature.featured == true %}
				{% include feature.html feature=feature %}
			{% endif %}
		{% endfor %}
	</div>
</div>


[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"