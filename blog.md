---
layout: page
title: Blog
description: "Artículos, lore y extras del mundo de 'La Leyenda de las Esferas'."
---

# Blog

Aquí encontrarás las últimas noticias, artículos sobre el mundo, desarrollo de personajes y mucho más.

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      <span class="post-meta">{{ post.date | date: "%d %b, %Y" }}</span>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>