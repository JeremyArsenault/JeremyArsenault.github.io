---
layout: page
title: Blog Title
tagline: Tagline
description: Description
---

landing (with posts!)

****************

# Hello

world!


****************

# Archive

{% for post in site.posts %}
  <article>
    <ul>
      <li>
        <a href="{{ post.url }}">
        {{ post.title }}
        </a><br>
        <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
      </li>
    </ul>
  </article>
{% endfor %}
