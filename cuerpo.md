---
layout: page
title: Cuerpo
update: 2025-02-18 18:57:00 -0600
---
Es la primer area a mejorar, si no sabes por donde empezar a crear tu mejor versión inicia haciendo ejercicio y mejorando tu alimentación. Una vez que domines tu cuerpo tendras la fuerza para dominar otras areas de tu vida.
<p>{% for post in site.categories["cuerpo"] %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>