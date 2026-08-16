---
permalink: /software/
title: Software
author_profile: false
---

## R Packages

### [mdgm](https://jbcart.github.io/mdgm/)

**Mixture of Directed Graphical Models** --- Bayesian inference for discrete
spatial random fields using mixtures of directed acyclic graphs. The package
provides MCMC sampling over DAG structures (spanning trees, acyclic
orientations) with optional emission models (Bernoulli, Gaussian, Poisson) for
hierarchical observation processes. Built with a C++20 core for efficient graph
algorithms and sampling.

- [Documentation](https://jbcart.github.io/mdgm/)
- [GitHub](https://github.com/jbcart/mdgm)
- [Paper (arXiv)](https://arxiv.org/abs/2406.15700)

Install from GitHub:
```r
# install.packages("pak")
pak::pak("jbcart/mdgm")
```
