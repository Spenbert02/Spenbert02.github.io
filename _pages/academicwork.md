---
layout: archive
# title: "Academic Work"
permalink: /academicwork/
author_profile: true
---


{% include base_path %}

# Papers

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
<br/><br/>

# Patents

{% for post in site.patents reversed %}
  {% include archive-single-patent.html %}
{% endfor %}
<br/><br/>

# Presentations

{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
