---
layout: base
---
<article class="post h-entry" itemscope itemtype="http://schema.org/BlogPosting">

  <header class="post-header">
    <h1 class="post-title p-name" itemprop="name headline">{{ page.title | escape }}</h1>
    <p class="post-meta">
      Update: {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      <time class="dt-published" datetime="{{ page.update | date_to_xmlschema }}" itemprop="datePublished">
        {{ page.update | date: date_format }}
      </time>
      {%- if page.modified_date -%}
        ~ 
        {%- assign mdate = page.modified_date | date_to_xmlschema -%}
        <time class="dt-modified" datetime="{{ mdate }}" itemprop="dateModified">
          {{ mdate | date: date_format }}
        </time>
      {%- endif -%}
      {%- if page.author -%}
        • {% for author in page.author %}
          <span itemprop="author" itemscope itemtype="http://schema.org/Person">
            <span class="p-author h-card" itemprop="name">{{ author }}</span></span>
            {%- if forloop.last == false %}, {% endif -%}
        {% endfor %}
      {%- endif -%}</p>
  </header>

  <div class="post-content e-content" itemprop="articleBody">
    {{ content }}
  </div>

  {%- if site.disqus.shortname -%}
    {%- include disqus_comments.html -%}
  {%- endif -%}

  <a class="u-url" href="{{ page.url | relative_url }}" hidden></a>
</article>

<hr><br>

<div class="PageNavigation">
  {% if page.previous.url %}
    <p><a class="prev" href="{{page.previous.url}}">&laquo; {{page.previous.title}}</a></p>
  {% endif %}

  {% if page.next.url %}
    <p align="right"><a class="next" href="{{page.next.url}}">{{page.next.title}} &raquo;</a></p>
  {% endif %}
</div>
<p align="center"><a rel="me" href="https://blog.zettahard.net/1-cuerpo.html">&laquo; Todos los posts sobre {{ page.category }} &raquo;</a></p>
<p align="center"><a rel="me" href="../../../../">&laquo; Todos los posts &raquo;</a></p>