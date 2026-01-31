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

- [ABCD Post]({{ site.baseurl }}/_posts/abcd.md)  
- [XYZ Post]({{ site.baseurl }}/_posts/xyz.md)
