{% for npc in site.npcs %}
<h2>{{ npc.fullname }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}