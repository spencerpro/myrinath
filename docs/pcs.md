---
title: Player Characters
---
{% for pc in site.pcs %}
<h2>{{ pc.fullname }}</h2>
<h3>{{ pc.species }} {{ pc.class }}</h3>
  <p>{{ pc.content | markdownify }}</p>
{% endfor %}