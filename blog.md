---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% if site.posts.size > 0 %}
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
        {% if post.excerpt %}
          <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>No posts available yet.</p>
{% endif %} 