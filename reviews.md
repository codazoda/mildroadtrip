---
layout: page
title: Reviews
permalink: /reviews/
---

<ul>
{% for post in site.posts %}
  {% if post.tags contains "review" %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>