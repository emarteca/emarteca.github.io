---
title: "ESM refactoring"
collection: ongoing_projects
excerpt: 'Refactoring NodeJS applications to automatically introduce ECMAScript Modules'
---

Refactoring NodeJS applications to automatically introduce ECMAScript Modules.
NodeJS introduced ECMAScript modules in 2015, which added many nice advantages such as more static guarantees, the ability for treeshaking and selective imports, etc.
However, many old packages were never modernized and still use old styles of creating modules and while newer code can interact with these packages they lose many of the advantages of the modern features.
With this refactoring, we generate the corresponding modern module from the old code when possible.


### Current status
This paper was rejected from ICSE 2021; we plan to resubmit to another venue once we address the reviewer concerns.