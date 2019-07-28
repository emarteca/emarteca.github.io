---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

Email me if you would like a pdf copy of any of the papers which are behind paywalls.

You can also find my articles on <span style="color:blue"><a href="https://scholar.google.ca/citations?user=JP-gFuQAAAAJ&hl=en">my Google Scholar profile</a></span>.

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
