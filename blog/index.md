---
layout: page
title: Blog
permalink: /blog/
---

# Blog Posts

{% for post in site.posts %}
<div class="post-preview">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
  {% if post.categories %}
    <div class="categories">
      {% for cat in post.categories %}
        <span class="category">{{ cat }}</span>
      {% endfor %}
    </div>
  {% endif %}
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url }}" class="read-more">Read more →</a>
</div>
{% endfor %}
