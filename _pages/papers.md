---
layout: archive
title: "Papers"
permalink: /papers/
author_profile: true
---


{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

---

# Patents

{% for post in site.patents reversed %}
  {% include archive-single-patent.html %}
{% endfor %}

---

# Presentations

{% for post in site.talks reversed %}
  {% include archive-single-talk.html show_excerpt=false %}
{% endfor %}

