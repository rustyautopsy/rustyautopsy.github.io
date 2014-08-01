---
layout: page
Title: Skills
---
<ul class="posts">
  {% assign posts = site.categories.skills | sort: 'title' %}
  {% for post in posts%}
  <li>
    <small class="datetime muted" data-time="{{ post.date }}">{{ post.date | date_to_string }} </small>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>

