---
bg: "music.jpeg"
layout: page
permalink: /Shorts/
title: "Shorts"
crawlertitle: "Shorts"
summary: "not the kind you wear"
active: personal
---
{% for post in site.posts limit: 5 %}
  {% if post.type == 'short' %}
<article class="index-page">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  {{ post.excerpt }}
</article>
  {% endif %}
{% endfor %}
