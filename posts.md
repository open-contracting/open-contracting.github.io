---
layout: home
title: Latest updates
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date  | date_to_string }}: {{ post.title }}</a> {% if post.author %} ({{post.author}}) {% endif %}
    </li>
  {% endfor %}
</ul>