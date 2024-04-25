---
title: Home
date: 2024-01-01
layout: default
tags: [primary, footer]
---
{% assign items = stylesheet | sort: 'landmarks' | reverse %}
{% for item in items %}
{% if item.landmarks-name %}
- **[{{ item.name }}]({{ item.website }})**: {{ item.landmarks }}% ({{ item.landmarks-name }}) - [Github]({{ item.github }})
{% endif %}
{% endfor %}