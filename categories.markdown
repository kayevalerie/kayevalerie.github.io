---
layout: page
title: Categories
lastmod: 2022-07-16T14:48:52.505Z
---

{% for cat in site.categories %}
  <h3>{{ cat[0] }}</h3>
  <ul>
    {% for post in cat[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
