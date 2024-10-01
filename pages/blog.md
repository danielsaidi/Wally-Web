---
id: blog
layout: default
title: Blog
permalink: /blog/
---

<h1>Blog</h1>

<div class="blog">
    {% include kankoda/tags/list.html tags=site.tags firstmost="releases" %}
    {% for post in site.posts %}
    {% include kankoda/blog/list-item.html post=post %}
    {% endfor %}
    {% include kankoda/tags/scripts.html %}
</div>