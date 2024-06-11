---
title: Welcome to my webpage
link-name: Home
date: 2024-01-01
layout: default
tags: [primary, footer]
---
### Stylesheet

How works the CSS stylesheet.

{% for i in collections[nav] %}
- [{{ i.data.title }}]({{ i.url }})
{% endfor %}