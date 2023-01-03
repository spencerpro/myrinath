---
title: Non-Player Characters
---
{% for npc in site.npcs %}
<details><summary><h2>{{ npc.fullname }}</h2></summary>
  <p>{{ npc.content | markdownify }}</p>
  {% if npc.mirrors %}Mirror: {{ npc.mirrors }}{% endif %}
</details>
{% endfor %}