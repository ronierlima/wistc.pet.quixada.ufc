---
layout: default
title: Palestras  
---

# Palestras 

{% assign sorted_pages = site.pages | sort:"order" %}
{% for node in sorted_pages %}
{% if page.categories contains 'palestra' %}
<div class="item"><h3><a href="{{ page.path}}">{{ page.title }}</a></h3></div>
    {{page.description}}
{% endif %}
{% endfor %}