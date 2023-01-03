---
title: Non-Player Characters
---
{% for npc in site.npcs %}
<h2>{{ npc.fullname }}</h2>
  <p>{{ npc.content | markdownify }}</p>
  {% if npc.mirrors %}Mirror: {{ npc.mirrors }}{% endif %}
  <hr/>
{% endfor %}