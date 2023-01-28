---
layout: page
title: Sitemaps
permalink: sitemaps
---
{% for list in site.pages %}
<a href="{{ list.url | relative_url }}">{{ list.title }}</a>
{% endfor %}