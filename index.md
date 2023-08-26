---
layout: page
---

{% for post in site.posts %}
  <article>
    <div style="width: 100%;">
        <div style="width: 75%; float: left;"> 
          <h3><a href="{{ post.url }}">
          {{ post.title }}
          </a></h3>
        </div>
        <div style="margin-left: 25%; height: 100%; text-align: right; vertical-align: bottom;">
          <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
        </div>
    </div>
  </article>
{% endfor %}
