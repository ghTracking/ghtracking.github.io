---
layout: default
permalink: /Metal_Oxides/
---
{% for page in site.Metal_Oxides %}
{% assign url_parts = page.url | split: '/' %}
{% assign name = url_parts | last %}
<a class="page-link" href="{{ page.url | relative_url }}">{{ page.title }}</a>
{% endfor %}