---
layout: page
title: Productividad
update: 2025-02-06 17:45:00 -0600
---
<ul>
  {% for post in site.categories["productividad"] %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>