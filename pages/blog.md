---
id: blog
layout: default
title: Blog
permalink: /blog/
---

<div class="searchbar-header">
  <h1>Blog</h1>
  {% include kankoda/search/searchbar class="discrete-dark" %}
</div>

<div class="blog">
    {% include kankoda/tags/tag-list.html tags=site.tags firstmost="releases" %}
    {% for post in site.posts %}
    {% include kankoda/blog/list-item.html post=post %}
    {% endfor %}
    {% include kankoda/tags/tag-scripts.html %}
</div>