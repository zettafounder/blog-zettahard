---
layout: page
title: Mente
update: 2025-02-18 23:39:00 -0600
---
Dicen que el hombre que logre dominar su mente, dominara el mundo. Esta no es una afirmación que sea literalmente cierta, pero si es verdad que aquel que domina su mente puede dominar su mundo.
<p>{% for post in site.categories["mente"] %}
    <a href="{{ post.url }}"><img width="auto" max-width="360px" src="{{ post.banner }}" alt="{{ post.title }}"/></a><br><br>
{% endfor %}</p>