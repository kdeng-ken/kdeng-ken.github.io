---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

<h2>University of Oxford</h2>
<hr>
{% assign undergrad_teaching = site.teaching | where: "category", "oxford" %}
{% for post in undergrad_teaching %}
  {% include archive-single-teaching.html %}
{% endfor %}

<h2>University of Cambridge</h2>
<hr>
{% assign grad_teaching = site.teaching | where: "category", "cambridge" %}
{% for post in grad_teaching %}
  {% include archive-single-teaching.html %}
{% endfor %}
