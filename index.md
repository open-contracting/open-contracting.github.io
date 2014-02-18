---
layout: default
title: Welcome to the Open Contracting Data Standard Project
---
<div class="post-title">
    <div class="row">
        <div class="col-md-4">
            <div class="block">
            <h1>Hello</h1>
            <p>Some text</p>
            </div>
        </div>
        <div class="col-md-4">
            <div class="block">
            <h1>Hello</h1>
            <p>Some text</p>
            </div>
        </div>
        <div class="col-md-4">
            <div class="block">
            <h1>Hello</h1>
            <p>Some text</p>
            </div>
        </div>
    </div>
</div>


<div id="posts">
    {% for post in site.posts %}
      <div class="post">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | post.content }}</p>
      </div>
    {% endfor %}
</div>
