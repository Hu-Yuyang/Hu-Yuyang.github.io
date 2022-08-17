---
permalink: /
layout: archive
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a incoming Ph.D. student in the <a href="https://cigroup.wustl.edu/">Computational Imaging Group</a> with the Department of ESE at Washington University in St. Louis. Before that, I received my Master's degree in Electrical Engineering at Washington University in St. Louis. My research advisor is <a href="https://cigroup.wustl.edu/ulugbek-s-kamilov/"> Prof. Ulugbek Kamilov</a>.

Currently, my research of interests include inverse problem, parallel MRI reconstruction, deep learning and large-scale optimization. 

<p>&nbsp;</p>

<h1> News </h1>
{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

<div style="display: none;">
  <h6>Page views:</h6>
  <a href="https://www.hitwebcounter.com" target="_blank">
  <img src="https://hitwebcounter.com/counter/counter.php?page=7680519&style=0007&nbdigits=5&type=page&initCount=0" title="Total Website Hits" Alt="Web Hits" border="0" /></a>
  <h6>Unique visitors</h6>
  <a href="https://www.hitwebcounter.com" target="_blank">
  <img src="https://hitwebcounter.com/counter/counter.php?page=7680520&style=0007&nbdigits=5&type=ip&initCount=0" title="Total Website Hits" Alt="Web Hits" border="0" /></a>
</div>
