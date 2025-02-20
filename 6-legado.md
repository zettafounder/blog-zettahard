---
layout: page
title: Legado
update: 2025-02-19 00:45:00 -0600
---
¿Qué es lo que quieres que los demás recuerden de ti?
{% assign i_posts = site.categories["legado"] | sort:"date" %}
<p>{% for post in i_posts %}
    <a href="{{ post.url }}"><img width="auto" max-width="360px" src="{{ post.banner }}" alt="{{ post.title }}"/></a><br><br>
{% endfor %}</p>