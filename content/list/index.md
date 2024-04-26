---
title: Lists
date: 2024-01-02
layout: default
tags: [primary, secondary]
aside: true
---
{% assign items = stylesheet | sort: 'landmarks' | reverse %}
{% for item in items %}
{% if item.landmarks-name %}
- **[{{ item.name }}]({{ item.website }})**: {{ item.landmarks }}% of HTML landmarks - [stylesheet](/assets/css/{{ item.name }}.css) - [Github]({{ item.github }})
{% endif %}
{% endfor %}