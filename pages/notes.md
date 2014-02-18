---
layout: single
title: Notes
---
#### Archive
* [Notes from our meeting in Montreal in Janaury 2014](workshops/2014-01-Montreal)

#### Updates Archive
<ul class="posts">
{% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
