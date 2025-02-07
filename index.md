---
layout: home
update: 2025-02-06 17:45:00 -0600
---

<h1>Ultimos posts</h1>

    {% for post in site.posts %}
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        {{ post.excerpt }}
    {% endfor %}

{% for post in site.posts %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    {{ post.excerpt }}
{% endfor %}