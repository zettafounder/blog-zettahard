---
layout: page
title: Cuerpo
update: 2025-02-18 18:57:00 -0600
---
Es la primer area a mejorar, si no sabes por donde empezar a crear tu mejor versión inicia haciendo ejercicio y mejorando tu alimentación. Una vez que domines tu cuerpo tendras la fuerza para dominar otras areas de tu vida.
{% assign i_posts = site.categories["cuerpo"] | sort:"date" %}
<p>{% for post in i_posts %}
    <a href="{{ post.url }}"><img width="auto" max-width="360px" src="{{ post.banner }}" alt="{{ post.title }}"/></a><br><br>
{% endfor %}</p>