---
title: Blog
layout: home
nav_order: 2   # This sets the sidebar order
---

# Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}
