---
bg: "piano.jpeg"
layout: page
title: "personal"
crawlertitle: "Personal thoughts"
permalink: /about/
summary: "Personal thoughts"
active: Personal
---

{% for post in site.posts limit: 5 %}
  {% if post.type is 'short' %}
    <article class="index-page">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </article>
  {}
{% endfor %}
