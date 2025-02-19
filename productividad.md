---
layout: page
title: 3. Productividad
update: 2025-02-06 17:45:00 -0600
---
Mucho de lo que se necesita para optimizar tu vida se encuentra aquí. Organización, planeación, administración, etc.
<p>{% for post in site.categories["productividad"] %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>