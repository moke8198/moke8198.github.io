---
bg: "music.jpeg"
layout: page
permalink: /Shorts/
title: "Shorts"
crawlertitle: "Shorts"
summary: "lighter topics (check back later)"
active: personal
---
{% for post in site.posts %}
  {% if post.type == 'short' %}
<article class="index-page">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  {{ post.excerpt }}
</article>
  {% endif %}
{% endfor %}
