---
title: Blog
layout: default
nav_order: 2
---

# Blog

## Featured Posts

{% assign abc_post = site.posts | where: "title", "ABCD Example Post" | first %}
{% assign xyz_post = site.posts | where: "title", "XYZ Example Post" | first %}

{% if abc_post %}
- [{{ abc_post.title }}]({{ abc_post.url }}) — {{ abc_post.date | date: "%b %-d, %Y" }}
{% endif %}

{% if xyz_post %}
- [{{ xyz_post.title }}]({{ xyz_post.url }}) — {{ xyz_post.date | date: "%b %-d, %Y" }}
{% endif %}

---

## All Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}
