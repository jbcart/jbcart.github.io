---
permalink: /research/
title: "Research"
author_profile: false
---

Most of the data behind real decisions is discrete: whether a shopper buys,
which item they choose, how a survey respondent rates something on a
five-point scale. My research develops models for these outcomes that scale
to large problems, stay interpretable, and are honest about their
uncertainty. The same toolkit has carried me from urban sociology to retail
assortment planning.

**Models for discrete data.** My core methodological interest is models for
discrete outcomes (binary, categorical, ordinal, and counts) that depend on
one another across space, networks, or a set of related choices. Classical
tools such as Gaussian processes and Markov random fields either scale poorly
to many locations (the "large n" problem) or break down when the response
itself is high-dimensional (the "large p" problem). Surveys are a good
example: they collect many discrete rating items per respondent, yet those
items are rarely modeled jointly, even though they share spatial and social
structure. My framework of mixtures of directed graphical models avoids the
intractable normalizing constants of undirected Markov random fields, and it
is the foundation I'm building on toward identifiable inference when n and p
are both large.

**Identifiability.** Many popular latent-variable models, such as spatial
generalized linear mixed models, are only partially identifiable: their
posteriors never concentrate on the truth, even with infinite data. I study
the assumptions that restore identifiability, including discrete latent
structure, sparsity, and hierarchical layering. In practice, this is the
question of what the data can and cannot tell you. Identifiability is what
lets a fitted model be *interpreted*, not just used to predict.

**Borrowing from machine learning, for inference rather than prediction.**
Deep learning is built on graphical models, with layers of latent variables
connected by a directed graph, and it uses ideas like sparsity-inducing
regularization to improve predictive accuracy. I adapt these concepts toward
a different end: understanding which constraints and induced sparsity on that
graph are needed for identifiability, so the resulting model supports
interpretation and valid uncertainty quantification.

**Applications.** My dissertation applied this framework to survey data from
the Adolescent Health and Development in Context (AHDC) study, developing a
land-use filtering model to spatially predict collective efficacy ratings in
an urban setting. At Hershey, the same ideas carry over to consumer choice:
discrete, high-dimensional data on what shoppers put in a basket, paired with
tractable optimization for assortment decisions. The domains differ, but the
underlying problem is the same: making sense of many interdependent discrete
choices.

## Where I want to go next

**Decision science for experimentation.** Most A/B testing is still framed as
hypothesis testing, and modern ML variants mostly answer the same question: is
the effect significant? Executives usually want to know something else: *what
is the risk of not shipping this?* Two toolkits answer that question more
directly.

Bayesian decision theory replaces the significance question with two
quantities: the posterior probability that a feature delivers incremental
lift, and the expected loss of shipping it versus holding it back. Recent work
extends this to many metrics at once, pooling information across them and
shrinking noisy ones, rather than relying on multiple-testing corrections that
are principled but raise the bar for detecting real effects. That matters
because business effects are often small but valuable: a 0.5% lift can be
worth millions of dollars.

E-values solve the monitoring problem. They measure cumulative evidence that
stays valid no matter how often you look, so a test can stop as soon as the
answer is clear. With no penalty for peeking, the statistician stops being the
scold guarding the false discovery rate and becomes a collaborator. E-values
can also be combined across tests while keeping formal error guarantees.

From what I've seen in the literature, applying formal decision theory to
business questions like these is still low-hanging fruit.

**New problems, approached like research.** I want to keep working where
challenging business problems push me to grow my technical toolkit. My PhD
trained me less in any one method than in how to take on a problem I haven't
seen before: dig into the literature, weigh the limitations, risks, and
tradeoffs of candidate models, and learn new techniques independently. I pair
that with building consensus on which question we actually need to answer, so
the effort goes into the right problem.
