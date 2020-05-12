---
layout: default
title: Minicursos   
---


# Minicursos 

{% assign sorted_pages = site.pages | sort:"order" %}
{% for node in sorted_pages %}
{% if page.categories contains 'minicurso' %}
<div class="item"><h3><a href="{{ page.path}}">{{ page.title }}</a></h3></div>
    {{page.description}}
{% endif %}
{% endfor %}