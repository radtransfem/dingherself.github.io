---
layout: default
posts_category: blog
title:  "Tags"
---

<h1>Tags</h1>

{% for tag in site.tags %}
  <h2 id="{{ tag[0] }}">{{ tag[0] | prepend: '#' }}</h2>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}" style="padding-right: 7px;">{{ post.title }}</a>{%- unless post.posts_category == "nodate" -%}<small class="text-body-secondary" style="font-style: italic;">{{ post.date | date: "%a, %b %e, %Y" }}{%- endunless -%}</small></li>
    {% endfor %}
  </ul>
{% endfor %}