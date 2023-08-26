---
layout: page
---

{% for post in site.posts %}
  <article>
    <h3><a href="{{ post.url }}">
    {{ post.title }}
    </a>
    <span style="font-size:16px;"><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></span>
    </h3>
  </article>
  <br>
{% endfor %}
