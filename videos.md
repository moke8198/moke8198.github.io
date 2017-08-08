---
bg: "music.jpeg"
layout: page
permalink: /music/
title: "music"
crawlertitle: "Music"
summary: "the universal language"
active: videos
---
 <table style="width:100%">
{% for post in site.posts %}
  {% if post.type == 'video' %}
<tr>
 <td><iframe width="420" height="315"
  src="{{ post.link }}">
  </iframe></td><td> {{ post.description }}</td>
</tr>
  {% endif %}
{% endfor %}
</table> 
