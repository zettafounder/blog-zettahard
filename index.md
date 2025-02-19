---
layout: home
update: 2025-02-06 17:45:00 -0600
---
Este no es solo un blog, es "el blog". Aquí esta toda la inormación que recopile por mucho tiempo, organice y compacte para que tú puedas ser mejor.

> Usa la información de este blog con responsabilidad.

<h1>Posts</h1>

<p>{% for post in site.posts %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>