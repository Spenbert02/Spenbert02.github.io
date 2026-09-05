---
title: "Posts"
permalink: /posts/
author_profile: true
---

{% include base_path %}

<ul class="post-list">
{% for post in site.posts %}
  <li class="post-list__item">
    <a class="post-list__link" href="{{ base_path }}{{ post.url }}">
      {% if post.header.teaser %}
        <img class="post-list__thumb" src="{{ post.header.teaser | prepend: '/images/' | prepend: base_path }}" alt="">
      {% endif %}
      <div class="post-list__body">
        <h2 class="post-list__title">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</h2>
        <p class="post-list__excerpt">{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
      </div>
    </a>
  </li>
{% endfor %}
</ul>
