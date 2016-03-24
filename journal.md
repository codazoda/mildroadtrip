---
layout: page
title: Journal
permalink: /journal/
---

<ul>
{% for post in site.posts %}
  {% if post.tags contains "journal" %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>