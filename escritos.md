---
layout: page
title: Escritos
---
{% assign i_escritos = site.escritos | sort:"date" | reverse %}

{% for escrito in i_escritos %}
  <h3><a href="{{ escrito.url }}">{{ escrito.title }}</a></h3><p class="post-meta"> {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <time class="dt-published" datetime="{{ escrito.date | date_to_xmlschema }}" itemprop="datePublished">
        {{ escrito.date | date: date_format }}
        </time>
        {%- if escrito.modified_date -%}
        ~ 
        {%- assign mdate = escrito.modified_date | date_to_xmlschema -%}
        <time class="dt-modified" datetime="{{ mdate }}" itemprop="dateModified">
            {{ mdate | date: date_format }}
        </time>
        {%- endif -%} - {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <time class="dt-published" datetime="{{ escrito.fin | date_to_xmlschema }}" itemprop="datePublished">
        {{ escrito.fin | date: date_format }}
        </time>
        {%- if escrito.modified_date -%}
        ~ 
        {%- assign mdate = escrito.modified_date | date_to_xmlschema -%}
        <time class="dt-modified" datetime="{{ mdate }}" itemprop="dateModified">
            {{ mdate | date: date_format }}
        </time>
        {%- endif -%}
  </p>
{% endfor %}