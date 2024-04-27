---
title: Tests
date: 2024-01-03
layout: default
tags: [primary]
aside: true
---
{% for item in collections.tests %}
- [{{ item.data.description }}]({{ item.url }})
{% endfor %}

## Tests with URL links
- [Drop-in Minimal CSS](/tests/dropin) | <a href="https://dohliam.github.io/dropin-minimal-css/" target="_new">Website demo</a>
- [HTML5 Elements Tester](/dropin/html5-elements-tester) | <a href="https://alexandersandberg.github.io/html5-elements-tester/" target="_new">Website demo</a>
- [% of semantic elements styled](/tests/semantic) | <a href="https://codepen.io/melissamcewen/embed/WNoweNg?default-tab=result&theme-id=15606" target="_new">Website code</a>
- [% of HTML5 elements styled](/tests/elements)
