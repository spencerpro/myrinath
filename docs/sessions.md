---
title: Sessions
---
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.url }}{{ post.url }}">{{ post.date | date: "%Y %B %d" }} {{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
