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

I am a second-year Master student in the <a href="https://cigroup.wustl.edu/">Computational Imaging Group</a> with the Department of ESE at Washington University in St. Louis. My research advisor is <a href="https://cigroup.wustl.edu/ulugbek-s-kamilov/"> Prof. Ulugbek Kamilov</a>.

Currently, my research of interests include inverse problem, parallel MRI reconstruction, deep learning and large-scale optimization. 

<p>&nbsp;</p>

<h1> News </h1>

{% include base_path %}
{% for post in site.posts %}
  {% include archive-single.html %}  
{% endfor %}
