---
title: Non-Player Characters
---
{% for npc in site.npcs %}
<h2>{{ npc.fullname }}</h2>
  <p>{{ npc.content | markdownify }}</p>
  {% if npc.mirrors }<p>Mirror Vol: {% for m in npc.mirrors %}{{ m }} {% endfor %}</p>{% endif }
  {% if npc.sessions }<p>Session: {% for session in npc.sessions %}{{ session }} {% endfor %}</p>{% endif }
  <hr/>
{% endfor %}