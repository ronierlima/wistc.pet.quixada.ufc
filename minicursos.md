---
layout: default
title: minicursos   
---

{% for page in site.pages %}
{% if page.categories contains 'minicurso' %}
<div class="item"><h3><a href="{{ page.path}}">{{ page.title }}</a></h3></div>
{% endif %}
{% endfor %}