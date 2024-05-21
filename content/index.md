---
title: Home
date: 2024-01-01
layout: default
tags: [primary, footer]
---
Stylesheet in use: {{ css }}.

### Best frameworks

{%- for item in stylesheet %}
{%- if item.landmarks > 80 %}
- [{{ item.name }}]({{ item.website }}): {{ item.remarks }}
{%- endif %}
{%- endfor %}

### Then...

{%- for item in stylesheet %}
{%- if item.landmarks < 80 %}
- [{{ item.name }}]({{ item.website }}): {{ item.remarks }}
{%- endif %}
{%- endfor %}