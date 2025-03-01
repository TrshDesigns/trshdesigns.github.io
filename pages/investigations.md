---
layout: page
title: Investigations
permalink: /investigations/
---

<ul>
  {% for investigation in site.investigations %}
    <li><a href="{{ investigation.url }}">{{ investigation.title }}</a></li>
  {% endfor %}
</ul>