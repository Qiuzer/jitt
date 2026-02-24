---
layout: default
title: "jitt 的空间"
---

## GitHub Pages

Self-taught iOS developer improving my English by building apps with SwiftUI.

---

## 文章列表

{% if site.posts.size > 0 %}
<ul>
  {% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - </span>
    <a href="{{ post.url | relative_url }}">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
    </a>
  </li>
  {% endfor %}
</ul>
{% else %}
暂时还没有文章，敬请期待。
{% endif %}
