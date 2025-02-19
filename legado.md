---
layout: page
title: 6. Legado
update: 2025-02-19 00:45:00 -0600
---
¿Qué es lo que quieres que los demás recuerden de ti?
<p>{% for post in site.categories["legado"] %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>