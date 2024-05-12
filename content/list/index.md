---
title: Lists
date: 2024-01-02
layout: default
tags: [primary]
aside: true
---
{% for item in collections.list %}
- [{{ item.data.title }}]({{ item.url }})
{% endfor %}

### Demo 1
<pre>
- banner
  - Primary (Navigation)
- Main
  - Demo (Region)
    - Complementary
      - Secondary (Navigation)
- Content information
  - Footer (Navigation)
</pre>
### Demo 2
<pre>
- banner
  - Primary (Navigation)
- Main
  - Demo (Region)
  - Complementary
    - Secondary (Navigation)
  - Article
- Content information
  - Footer (Navigation)
</pre>
### Demo 3
<pre>
- banner
  - Primary (Navigation)
- Main
  - Complementary
    - Secondary (Navigation)
  - Demo (Region)
  - Article
- Content information
  - Footer (Navigation)
</pre>
