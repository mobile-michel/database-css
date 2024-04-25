---
title: Lists
date: 2024-01-02
layout: default
tags: [primary]
---
{% for post in collections.list %}
- [{{ post.data.title }}]({{ post.url }})
{% endfor %}