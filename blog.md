---
title: Blog
layout: default
nav_order: 2
---

# Blog

## Direct Links to Key Posts

{% assign abc_post = site.posts | where: "title", "ABCD Example Post" | first %}
{% assign xyz_post = site.posts | where: "title", "XYZ Example Post" | first %}

- [{{ abc_post.title }}]({{ abc_post.url | prepend: site.baseurl }})
- [{{ xyz_post.title }}]({{ xyz_post.url | prepend: site.baseurl }})
