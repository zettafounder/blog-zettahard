---
layout: page
title: Productividad
update: 2025-02-06 17:45:00 -0600
---
<p>{% for post in site.categories["productividad"] %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}</p>