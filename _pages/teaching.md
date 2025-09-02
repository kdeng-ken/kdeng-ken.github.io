---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

<h2>University of Oxford</h2>
<hr>
{% assign ox_teaching = site.teaching | where: "category", "oxford" %}
{% for post in ox_teaching %}
  {% include archive-single-teaching.html %}
{% endfor %}

<h2>University of Cambridge</h2>
<hr>
{% assign cam_teaching = site.teaching | where: "category", "cambridge" %}
{% for post in cam_teaching %}
  {% include archive-single-teaching.html %}
{% endfor %}
