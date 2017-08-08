---
bg: "music.jpeg"
layout: page
permalink: /videos/
title: "Videos"
crawlertitle: "Videos"
summary: "Videos"
active: videos
---
{% for post in site.posts %}
  {% if post.type == 'video' %}
 <iframe width="420" height="315"
src="{{ post.link }}">
</iframe> {{ post.description }}
  {% endif %}
{% endfor %}
