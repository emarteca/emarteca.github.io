---
title: "The effects of computational resources on flaky tests"
collection: publications
excerpt: 'A tool for automatic identification of Resource-Affected Flaky tests (in Java, Python, and JavaScript code bases), and reporting resource configurations in which tests are (most) stable.'
date: 2023-10-18
venue: 'In submission to IEEE TSE'
---

<a href='https://arxiv.org/pdf/2310.12132.pdf'>Access preprint here</a>

Flaky tests are tests that nondeterministically pass and fail in unchanged code. These tests can be detrimental to developers’ productivity. Particularly when tests run in continuous integration environments, the tests may be competing for access to limited computational resources (CPUs, memory etc.), and we hypothesize that resource (in)availability may be a significant factor in the failure rate of flaky tests. 

This paper presents an assessment of the impact that computational resources have on flaky tests, from a set of projects in Java, JavaScript and Python, over a set of 27 different resource configurations.
We also do automatic identification of RAFTs (Resource-Affected Flaky Tests), and determination of which resource configurations avoid the RAFTs.
Together, this information encompasses a tool for developers to identify RAFTs in their code, and report configurations in which their tests are stable.


Recommended citation: Denini Silva, Martin Gruber, Satyajit Gokhale, Ellen Arteca, Alexi Turcotte, Marcelo d’Amorim, Wing Lam, Stefan Winter, and Jonathan Bell.	"The effects of computational resources on flaky tests." <i>In submission to IEEE TSE</i>, 2023.