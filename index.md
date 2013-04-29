---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts limit 10 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    {{ post.content | strip_html | truncatewords:75 }}
    <a href="{{ post.url }}">Read more...</a>
    </li>
  {% endfor %}
</ul>
