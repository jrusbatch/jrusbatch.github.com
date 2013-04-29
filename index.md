---
layout: default
---
{% include JB/setup %}

<div class="page-header">
  <h1>Posts</h1>
</div>

<ul class="posts">
  {% for post in site.posts %}
    <li class="post">
      <span class="post-timestamp">{{ post.date | date_to_string }}</span>
      <a class="post-title" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
