---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a second-year Master student in the <a href="https://cigroup.wustl.edu/">Computational Imaging Group</a> with the Department of ESE at Washington University in St. Louis. My research advisor is <a href="https://cigroup.wustl.edu/ulugbek-s-kamilov/"> Prof. Ulugbek Kamilov</a>.

Currently, my research of interests include inverse problem, Parallel image, deep learning and large-scale optimization. 

<p>&nbsp;</p>

<h1> News </h1>

{% include base_path %}
{% capture 2021 %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

