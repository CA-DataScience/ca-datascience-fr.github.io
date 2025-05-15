---
layout: page
title: "Blog"
permalink: "/blog/"
header:
  image_fullwidth: header_blog.jpg
---

<div class="row">
<div class="medium-8 medium-push-2 columns">
<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
      <p>
        {{ post.excerpt | strip_html | truncatewords: 50 }}
      </p>
      <a href="{{ post.url | relative_url }}" class="button small radius">Read more</a>
    </li>
  {% endfor %}
</ul>
</div>
</div>