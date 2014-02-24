---
layout: single
title: Site List
---
### Pages
<ul>
{% assign pages_list = site.pages %}
{% include JB/pages_list %}
</ul>

### Posts
<ul>
{% assign pages_list = site.posts %}
{% include JB/pages_list %}
</ul>
