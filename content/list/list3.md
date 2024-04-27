---
title: Lists
description: list by landmarks score
date: 2024-02-03
layout: default
tags: [list, secondary]
aside: true
---
{% assign items = stylesheet | sort: 'landmarks' | reverse %}
{% for item in items %}
{% if item.landmarks-name %}
- **[{{ item.name }}]({{ item.website }})**: [{{ item.landmarks }}% landmarks](/list/demo1/{{ item.name | slugify | url }}) | [{{ item.html-elements }}% elements](/list/demo1/{{ item.name | slugify | url }}) - [stylesheet](/assets/css/{{ item.name }}.css) - [Github]({{ item.github }})
{% endif %}
{% endfor %}