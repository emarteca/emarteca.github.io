---
layout: archive
title: "Ongoing Projects"
permalink: /ongoing_projects/
author_profile: true
---

This is an overview of my main ongoing projects that are not yet in paper form.

{% include base_path %}

{% for post in site.ongoing_projects reversed %}
  {% include archive-single.html %}
{% endfor %}
