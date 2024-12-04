---
layout: page
title: Escritos
---
{% assign i_escritos = site.escritos | sort:"date" | reverse %}

{% for escrito in i_escritos %}
  <h3><a href="{{ escrito.url }}">{{ escrito.title }}</a></h3>
{% endfor %}