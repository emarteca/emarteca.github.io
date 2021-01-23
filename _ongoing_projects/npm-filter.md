---
title: "npm-filter"
collection: ongoing_projects
excerpt: 'Tool for automatic analysis of a NodeJS JavaScript project: determine build/test commands, number of tests, number of failing tests, run CodeQL static analysis code over the project, ...'
---

Tool for automatic analysis of a JavaScript project: determine build/test commands, number of tests, number of failing tests, run CodeQL static analysis code over the project, ...

There are several main use cases:
* generate metadata for one project to determine what the relevant commands are
* analyze a collection of projects in order to identify candidate projects for a tool evaluation
* analyze a (large) collection of projects and analyze the trends in metadata

### Current status
The tool is working and currently being used internally to find candidate projects for evaluating other program analyses.
We're still working on a large-scale analysis of npm, with the end goal of presenting a study on the state of the NodeJS ecosystem, and maybe hosting a parallel site to npm where users can search for packages matching certain criteria (e.g., packages with at least 10 passing tests, etc.).