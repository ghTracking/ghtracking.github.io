---
layout: default
permalink: /X-ray_spectroscopy/
---
{% for page in site.X-ray_spectroscopy %}
{% assign url_parts = page.url | split: '/' %}
{% assign name = url_parts | last %}
<a class="page-link" href="{{ page.url | relative_url }}">{{ page.title }}</a>
{% endfor %}