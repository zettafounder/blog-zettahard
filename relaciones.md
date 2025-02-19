---
layout: page
title: 5. Relaciones
update: 2025-02-19 01:15:00 -0600
---
Dicen que eres lo que los demás recuerdan de ti y es lo que prentendo mejorar, quiero ser alguien que guste, alguien admirable y alguien en quien se pueda confiar.

Ser mejor hijo, pareja, hermano, amigo, padre, compañero.
<p>{% for post in site.categories["relaciones"] %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>