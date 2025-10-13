---
layout: page
title: Topics
permalink: /topics/
---

Browse by topic:

<ul>
{% assign cats = site.categories | sort %}
{% for cat in cats %}
  <li><a href="/topics/{{ cat[0] | slugify }}/">{{ cat[0] }} ({{ cat[1].size }})</a></li>
{% endfor %}
</ul>
