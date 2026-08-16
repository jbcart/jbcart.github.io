---
permalink: /research/
title: "Research"
author_profile: false
---

**Spatial models for discrete data.** My core methodological interest is
developing statistical models for spatially- or network-dependent discrete
outcomes — counts, ordinal responses, categorical and binary data — where
classical tools (Gaussian processes, Markov random fields) either scale poorly
to many locations (the "large n" problem) or break down when the response
itself is high-dimensional (the "large p" problem), as with survey instruments
that collect many discrete rating items per respondent, which are rarely
modeled jointly despite sharing spatial and social structure. My mixtures of
directed graphical models framework — an alternative to the intractable
normalizing constants of undirected Markov random fields — is one example of
this approach, and a foundation I'm building on toward identifiable inference
in this joint large-n, large-p regime.

**Identifiability.** A throughline across this work is identifiability: many
popular latent-variable spatial models (e.g., spatial generalized linear mixed
models) are only partially identifiable, so their posteriors never concentrate
on the truth even with infinite data. I study the assumptions — discreteness
of latent structure, sparsity, hierarchical layering — that restore
identifiability, since identifiable models are what let a fitted model be
*interpreted*, not just used to predict.

**Borrowing from machine learning, for inference rather than prediction.**
Deep learning relies heavily on graphical models — layers of latent variables
connected by a directed graph — using representation-learning ideas like
sparsity-inducing regularization to improve predictive accuracy. My goal is to
adapt these same concepts toward a different end: understanding what
constraints and induced sparsity on that graphical structure are necessary for
identifiability, so the resulting model supports interpretation and valid
uncertainty quantification rather than just prediction.

**Applications.** My dissertation applied this framework to survey data from
the Adolescent Health and Development in Context (AHDC) study, developing a
land-use filtering model for spatially predicting collective efficacy ratings
in an urban setting. My current work at Hershey extends the same ideas to a
new domain: pairing consumer choice models — discrete, high-dimensional data
on what shoppers put in a basket — with tractable optimization for assortment
decisions.
