---
title: Documentation
link-name: Doc
description: This is documentation.
date: 2024-01-02
tags: ["primary", "footer"]
---
{% for post in collections.doc %}
- [{{ post.data.title }}]({{ post.url | url }}) published on {{ post.data.date | date: '%d  %b %Y' }}, source is {{ post.data.author }}
{% endfor %}

### Test



{% for i in collections[navigation] %}
- [{{ i.data.title }}]({{ i.url }})
{% endfor %}