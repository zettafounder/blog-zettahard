---
layout: page
title: Legado
update: 2025-02-19 00:45:00 -0600
---
¿Qué es lo que quieres que los demás recuerden de ti?
<p>{% for post in site.categories["legado"] %}
    <a href="{{ post.url }}"><img width="auto" max-width="360px" src="{{ post.banner }}" alt="{{ post.title }}"/></a>
{% endfor %}</p>