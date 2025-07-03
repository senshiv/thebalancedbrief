---
# the default layout is 'page'
title: Blogs
icon: fas fa-pen-nib
order: 4
---

# 📝 Balanced Brief – Where Passion Meets Profession

Following pages include blogs on various categories.

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "blog" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>({{ post.date | date: "%Y-%m-%d" }})</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>
