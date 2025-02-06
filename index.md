---
layout: home
update: 2025-02-06 17:45:00 -0600
---

<h1>Latest Posts</h1>

<ul>
  {% for post in site.productividad %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>