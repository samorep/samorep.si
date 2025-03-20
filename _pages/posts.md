---
layout: page
title: "Zapisi"
description: "Terapevtske teme in osebna rast"
permalink: /posts/
background: '/assets/img/bg-post.jpg'
---

{% for post in site.posts %}

<article class="post-preview">
  <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
    <h2 class="post-title">{{ post.title }}</h2>
    {% if post.subtitle %}
    <h3 class="post-subtitle">{{ post.subtitle }}</h3>
    {% endif %}
  </a>
  <p class="post-meta">Objavljeno 
    {% assign m = post.date | date: "%-m" %}
    {{ post.date | date: "%-d." }}
    {% case m %}
      {% when '1' %}januarja
      {% when '2' %}februarja
      {% when '3' %}marca
      {% when '4' %}aprila
      {% when '5' %}maja
      {% when '6' %}junija
      {% when '7' %}julija
      {% when '8' %}avgusta
      {% when '9' %}septembra
      {% when '10' %}oktobra
      {% when '11' %}novembra
      {% when '12' %}decembra
    {% endcase %}
    {{ post.date | date: "%Y" }}
  </p>
</article>

<hr>

{% endfor %} 