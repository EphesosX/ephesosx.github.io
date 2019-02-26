---
layout: page
title: Research
published: true
---

My research interests include subgraph isomorphism, network science, iterative linear system solvers, machine learning, and image processing.

###### Publications

{% for publication in site.data.publications %}
* {% for name in publication.authors %}{% if name == publication.my_name %}**{{ name }}**{% else %}{{ name }}{% endif %}, {% endfor %}"[*{{ publication.title }}.*]({{ publication.url }})" {{ publication.venue }}
{% endfor %}
