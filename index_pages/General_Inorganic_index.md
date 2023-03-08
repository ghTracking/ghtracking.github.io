---
layout: default
permalink: /General_Inorganic/
---
{% for page in site.General_Inorganic %}
{% assign url_parts = page.url | split: '/' %}
{% assign name = url_parts | last %}
<a class="page-link" href="{{ page.url | relative_url }}">{{ page.title }}</a>
{% endfor %}