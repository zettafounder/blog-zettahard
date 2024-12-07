---
layout: home
update: 2024-12-03 22:00:00 -0600
---

> Escritos es un conjunto de notas que tome mientras me reconstruia, son conceptos que me ayudarón a salir "del hoyo" y decidi compartirlos con la esperanza de que le sirvan a alguien más.

{% assign i_escritos = site.escritos %}

{% for escrito in i_escritos | limit: 15 %}
  <a href=".{{ escrito.url }}">{{ escrito.title }}</a>
{% endfor %}
