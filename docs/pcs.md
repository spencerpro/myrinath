---
title: Player Characters
---
<dl>
{% for pc in site.pcs %}
<dt>{{ pc.fullname }}</dt>
<dl>{{ pc.species }} {{ pc.class }}</dl>
<dl>{{ pc.content | markdownify }}</dl>
{% endfor %}
</dl>