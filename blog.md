---
title: Blog
layout: home
nav_order: 2   # This sets the sidebar order
---

# Blog Posts

## All Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}

---

## Direct Links to Key Posts

{% assign abc_post = site.posts | where: "title", "ABCD Example Post" | first %}
{% assign xyz_post = site.posts | where: "title", "XYZ Example Post" | first %}

- [ABCD Example Post]({{ abc_post.url }})
- [XYZ Example Post]({{ xyz_post.url }})


