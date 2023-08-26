---
layout: page
---

{% for post in site.posts %}
  <article>
    <div style="width: 100%;">
        <div style="width: 75%; height: 60px; float: left;"> 
          <h3><a href="{{ post.url }}">
          {{ post.title }}
          </a></h3>
        </div>
        <div style="margin-left: 75%; height: 40px; display: flex;">
          <span style="align-self: flex-end; width: 100%; text-align: right; "><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></span>
        </div>
    </div>
  </article>
{% endfor %}
