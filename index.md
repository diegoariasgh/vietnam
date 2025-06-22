---
layout: default
title: "Vietnam June-July 2025"
---

Select a city to see photos from the trip:

<ul>
  {% assign cities = site.pages 
       | where_exp:"p","p.layout == 'city'" 
       | sort: "order" %}
  {% for page in cities %}
    <li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>
