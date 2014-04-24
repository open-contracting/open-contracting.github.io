---
layout: home
title: Blog posts
---
## Blog posts

You can keep in touch day-to-day with our work in progress through [the mailing list, github and twitter feeds](/pages/community.html). However, every now and then we will report on what's been going on during the standard development through short blog posts here.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date  | date_to_string }}: {{ post.title }}</a> {% if post.author %} ({{post.author}}) {% endif %}
    </li>
  {% endfor %}
</ul>


You can subscribe to a [feed of the latest posts here](/feed.xml). 