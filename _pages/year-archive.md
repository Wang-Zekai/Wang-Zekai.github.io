---
title: "博客"
permalink: /blog/
layout: single
author_profile: true
---

{% for post in site.posts %}
{% if post.tags contains "ICS" or post.tags contains "ics" %}
<article class="archive__item">
  <h2 class="archive__item-title">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h2>
  <p class="page__meta">{{ post.date | date: "%Y-%m-%d" }}</p>
  {% if post.excerpt %}
    <p class="archive__item-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
  {% endif %}
</article>
{% endif %}
{% endfor %}
