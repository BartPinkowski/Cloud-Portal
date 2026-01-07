---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% for post in site.posts %}
<div class="card">
  <strong><a href="{{ post.url | relative_url }}">{{ post.title }}</a></strong>
  <p>{{ post.date | date: "%Y-%m-%d" }} · {{ post.excerpt | strip_html | truncate: 160 }}</p>
</div>
{% endfor %}
