---
layout: home
update: 2024-12-03 22:00:00 -0600
---

## Escritos

{% assign i_escritos = site.escritos %}

{% for escrito in i_escritos | limit: 5 %}
  <a href=".{{ escrito.url }}">{{ escrito.title }}</a>
{% endfor %}

[Todos los posts](/escritos.html)

## Desafíos
