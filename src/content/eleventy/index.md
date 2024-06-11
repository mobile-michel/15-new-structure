---
title: Eleventy is my SSG
link-name: 11ty
description: This is some information about 11ty static site generator.
date: 2024-01-02
tags: ["primary", "footer"]
eleventyComputed:
    test: '{{ navigation }}'
---
{% for post in collections.eleventy %}
- [{{ post.data.title }}]({{ post.url | url }}) published on {{ post.data.date | date: '%d  %b %Y' }}, source is {{ post.data.author }}
{% endfor %}

Le texte: {{ test }} doit apparaître...