---
title: "Stubbifier"
collection: ongoing_projects
excerpt: 'Debloating JavaScript applications by identifying untested code through a callgraph analysis and replacing this code with stubs to dynamically load the code if needed.'
---

Debloating JavaScript applications by identifying untested code through a callgraph analysis and replacing this code with stubs to dynamically load the code if needed.
Since the code has the option of being dynamically loaded (i.e., it is not entirely removed) we can be much more aggressive with the debloating than traditional bundling tools -- these need to be soundly sure the code is dead, which is rarely true in a highly dynamic language like JavaScript.

Additionally, we implemented an optional "guarded execution mode", where a specified list of functions labelled dangerous (such as `eval` and `exec`, that execute arbitrary code) are flagged if they are executed in dynamically loaded code.
The idea is that since this code is untested it might contain some security vulnerabilities; indeed, in our evaluation we found several instances of packages with hardcoded dependencies on versions of libraries with problem calls to `eval`. 

### Current status
This paper was rejected from ICSE 2021; we hope to resubmit to another venue soon.