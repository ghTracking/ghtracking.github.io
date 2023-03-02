---
layout: default
permalink: /C_Courses/
---
{% for page in site.C_Courses %}
{% assign url_parts = page.url | split: '/' %}
{% assign name = url_parts | last %}
<a class="page-link" href="{{ page.url | relative_url }}">{{ page.title }}</a>
{% endfor %}