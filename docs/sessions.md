---
title: Sessions
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y %B %d" }} {{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
