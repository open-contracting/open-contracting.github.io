---
layout: single
title: Notes
date: 23/02/2014
---
This is where we keep links to notes from meetings, presentations, etc. that are going on.
If you think we've missed something, please [contact us](/pages/community.html).

We also have a [hackpad space](https://opencontractingdata.hackpad.com/) where we take live notes. We will try to
also document and record things here.

* [Use Cases](/pages/usecases/) developed through ongoing consultation
* [Datasets](datasets) that we have been analyzing
* [Personas](workshops/2014-01-Montreal/personas.html) that came out of the Montreal workshop
* [Notes](workshops/2014-01-Montreal) from our first OCDS workshop in Montreal - 31 January 2014
* [Hackpad](https://devchallenge.hackpad.com/Challenge-F1-Open-Contracting-WZSKzabvK3c) from the OCDS Development Challenge 27 & 28 January 2014
* [The initial sprint work in March 2013](firstsprint.html)

### Updates

<ul class="posts">
{% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
