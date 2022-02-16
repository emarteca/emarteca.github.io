---
title: "Stubbifier: Debloating Dynamic JavaScript Applications"
collection: publications
excerpt: 'Debloating JavaScript applications by identifying untested code via a callgraph analysis, and replacing this code with stubs to dynamically load it if needed.'
date: 2022-12-30
venue: 'ESME'
custom_tag: 'In revisions at'
---

<a href='http://emarteca.github.io/files/emse22.pdf'>Access preprint here</a>

Debloating JavaScript applications by identifying untested code via a callgraph analysis and replacing this code with stubs to dynamically load it if needed.
Since the code has the option of being dynamically loaded (i.e., it is not entirely removed) we can be much more aggressive with the debloating than traditional bundling tools -- these need to be soundly sure the code is dead, which is rarely true in a highly dynamic language like JavaScript.

Additionally, we implemented an optional "guarded execution mode", where a specified list of functions labelled dangerous (such as `eval` and `exec`, that execute arbitrary code) are flagged if they are executed in dynamically loaded code.
The idea is that since this code is untested it might contain some security vulnerabilities; indeed, in our evaluation we found several instances of packages with hardcoded dependencies on versions of libraries with problem calls to `eval`. 

Recommended citation: Turcotte, Alexi and Arteca, Ellen, Ashish Mishra, Saba Alimadadi, and Frank Tip. "Stubbifier: Debloating Dynamic JavaScript Applications." <i>In submission to Empirical Software Engineering</i> (2022).
