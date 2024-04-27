---
title: Lists
date: 2024-01-02
layout: default
tags: [primary]
aside: true
---
{% for item in collections.list %}
- [{{ item.data.description }}]({{ item.url }})
{% endfor %}