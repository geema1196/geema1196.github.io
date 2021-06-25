---
title: Home
layout: home
permalink: /
---


# A Simple Test Website

A link to another page:

- [About](/about/)

{% for post in site.posts %}
    {% assign title_slugged = post.title | slugify %}
    {% assign categories_current = post.categories | join: "/" %}
    - [{{ post.title }}](/blog/{{categories_current}}/{{title_slugged}}/)
{% endfor %}
