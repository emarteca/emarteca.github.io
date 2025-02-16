---
layout: archive
title: "Ongoing Projects"
permalink: /ongoing_projects/
author_profile: true
---

As part of my job, I work on the open-source tool [Diplomat](https://github.com/rust-diplomat/diplomat). This is a Rust tool for generating FFI bindings between Rust and other languages. 

My work has focused on interop between Rust and Kotlin. I also added support for callbacks and traits in the HIR (with full support implemented in the C and Kotlin backends).

{% include base_path %}

{% for post in site.ongoing_projects reversed %}
  {% include archive-single.html %}
{% endfor %}
