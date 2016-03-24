---
layout: page
title: Motorcycle
permalink: /motorcycle/
---

<ul>
{% for post in site.posts %}
  {% if post.tags contains "motorcycle" %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>