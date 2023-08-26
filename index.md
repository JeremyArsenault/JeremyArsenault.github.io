---
layout: page
---

{% for post in site.posts %}
  <article>
    <h3><a href="{{ post.url }}">
    {{ post.title }}
    </a>
    <span style="font-size:16px;text-align:right;"><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></span>
    </h3>
  </article>
{% endfor %}
