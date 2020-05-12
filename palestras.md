---
layout: default
title: Palestras  
---

# Palestras 


{% for page in site.pages %}
{% if page.categories contains 'palestra' %}
<div class="item"><h3><a href="{{ page.path}}">{{ page.title }}</a></h3></div>
    {{page.description}}
{% endif %}
{% endfor %}