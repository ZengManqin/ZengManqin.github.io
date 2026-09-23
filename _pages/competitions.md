---
layout: archive
title: "Competitions"
permalink: /competitions/
author_profile: true
---

{% for post in site.competitions reversed %}
  {% include archive-single.html %}
{% endfor %}
