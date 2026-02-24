---
layout: default
title: "Home"
---

## Posts

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
  <li class="post-list-item">
    <a class="post-list-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <a class="post-list-date" href="{{ post.url | relative_url }}">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
    </a>
  </li>
  {% endfor %}
</ul>
{% else %}
No posts yet.
{% endif %}
