---
title: Non-Player Characters
---
{% for npc in site.npcs %}
<h2>{{ npc.fullname }}</h2>
  <p>{{ npc.content | markdownify }}</p>
{% endfor %}