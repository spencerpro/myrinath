---
title: Non-Player Characters
---
{% for npc in site.npcs %}
{% if npc.image %}![NPC Image]({{ npc.image | relative_url | uri_escape }}){% endif %}
<details><summary><h2>{{ npc.fullname }}</h2></summary>
  <p>{{ npc.content | markdownify }}</p>
  <p>{% if npc.sessions %}Session: {{ npc.sessions }}{% endif %}</p>
  <p>{% if npc.mirrors %}Mirror: {{ npc.mirrors }}{% endif %}</p>
</details>
<hr/>
{% endfor %}