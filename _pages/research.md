---
permalink: /
title: "Research"
author_profile: true
redirect_from:
  - /about/
  - /about.html
  - /projects/
  - /papers/
---

{% include base_path %}

## Bio

I'm a PhD student in the <a href="https://cims.nyu.edu/gcl/people.html" target="_blank">Geometric Computing Lab</a> in the Courant Institute of Mathematical Sciences at NYU, working on geometry processing for medical image simulations. I was previously a staff researcher and undergraduate assistant in the <a href="https://sites.google.com/view/mcalpineresearchgroup/home" target="_blank">3D Printing Functional Materials and Devices Lab</a> at the University of Minnesota, where I worked on path planning algorithms for 3D bioprinting.

## Projects

<ul class="project-grid">
{% assign projects = site.portfolio | sort: 'order' %}
{% for post in projects %}
  {% unless post.hidden %}
  <li class="project-grid__item">
    <a class="project-grid__link" href="{{ base_path }}{{ post.url }}">
      {% if post.header.teaser %}
        <img class="project-grid__thumb" src="{{ post.header.teaser | prepend: '/images/' | prepend: base_path }}" alt="">
      {% endif %}
    </a>
    <span class="project-grid__title">{{ post.title | markdownify | remove: "<p>" | remove: "</p>" }}</span>
    {% if post.codeurl %}
      <a class="project-grid__subtitle" href="{{ post.codeurl }}" target="_blank">Code</a>
    {% endif %}
  </li>
  {% endunless %}
{% endfor %}
</ul>

## Works

{% assign works = site.publications | concat: site.patents | concat: site.talks %}
{% assign works = works | sort: 'date' | reverse %}
{% for post in works %}
  {% include archive-single-work.html %}
{% endfor %}
