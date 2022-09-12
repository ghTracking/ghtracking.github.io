I decided that it would be useful to practise making a page for a new set of notes.

At this point, I do need to remind myself of how collections work, but for now I shall list the 'quick fix' to prevent every page in the new folder from showing in the header.

Within `header.html`, there is the following structure:
```
    {%- if page_paths -%}
  <div class="trigger">
    {% for collection in site.collections %}
    {% if collection.label contains 'Mathematical_Methods' or collection.label contains 'practical_skills' or collection.label contains 'posts' %}
    {% else %}
    {% for page in site.[collection.label]] %}
    {% assign url_parts = page.url | split: '/' %}
    {% assign name = url_parts | last %}
    <a class="page-link" href="{{ page.url | relative_url }}">{{ name }}</a>
    {% endfor %}
    {% endif %}
    {% endfor %}
    <a class="page-link" href="{{ "/Mathematical_Methods" | relative_url }}"> Mathematical Methods </a>
    <a class="page-link" href="{{ "/practical_skills" | relative_url }}"> Practical Skills </a>
    {% endif %}
  </div>
```
In the above example, there are .md files within the folders `_Mathematical_Methods` and `_practical_skills`. Have I therefore done this without creating these folders as a collection? Unsure.

Being unsure, I also added
```
  Statistics:
    output: true
    permalink: /Statistics/:path/
```
into the _config.yml

Once the `{%if collection.label contains '###_### %}` is modified to include another `or` for a new folder