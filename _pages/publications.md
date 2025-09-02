---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2>Working Papers</h2>
<hr>
{% assign working_pubs = site.publications | where: "category", "working" | sort: "date" | reverse %}
{% for post in working_pubs %}
  {% include archive-single.html %}
{% endfor %}

<h2>Work in Progress</h2>
<hr>
{% assign progress_pubs = site.publications | where: "category", "progress" | sort: "date" | reverse %}
{% for post in progress_pubs %}
  {% include archive-single.html %}
{% endfor %}
