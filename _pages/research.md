---
permalink: /research/
title: "Research"
author_profile: false
---

Most of the data that drives real decisions is discrete: whether a shopper
buys, which item they choose, how a survey respondent rates something on a
five-point scale. My research develops models for these outcomes that scale
to large problems, stay interpretable, and are honest about their
uncertainty. The same toolkit has carried me from urban sociology to retail
assortment planning.

**Models for discrete data.** My core methodological interest is statistical
models for discrete outcomes (binary, categorical, ordinal, and counts) that
depend on one another across space, networks, or a set of related choices.
Classical tools such as Gaussian processes and Markov random fields either
scale poorly to many locations (the "large n" problem) or break down when the
response itself is high-dimensional (the "large p" problem). Survey instruments
are a good example: they collect many discrete rating items per respondent,
yet those items are rarely modeled jointly despite sharing spatial and social
structure. My mixtures of directed graphical models framework, an alternative
to the intractable normalizing constants of undirected Markov random fields,
is one answer, and a foundation I'm building on toward identifiable inference
when n and p are both large.

**Identifiability.** A throughline across this work is identifiability: many
popular latent-variable models (e.g., spatial generalized linear mixed
models) are only partially identifiable, so their posteriors never concentrate
on the truth even with infinite data. I study the assumptions that restore
identifiability, such as discreteness of latent structure, sparsity, and
hierarchical layering. In practice this is the question of what the data can
and cannot tell you, and identifiable models are what let a fitted model be
*interpreted*, not just used to predict.

**Borrowing from machine learning, for inference rather than prediction.**
Deep learning relies heavily on graphical models, with layers of latent
variables connected by a directed graph, and uses representation-learning
ideas like sparsity-inducing regularization to improve predictive accuracy. My
goal is to adapt these same concepts toward a different end: understanding
what constraints and induced sparsity on that graphical structure are
necessary for identifiability, so the resulting model supports interpretation
and valid uncertainty quantification rather than just prediction.

**Applications.** My dissertation applied this framework to survey data from
the Adolescent Health and Development in Context (AHDC) study, developing a
land-use filtering model for spatially predicting collective efficacy ratings
in an urban setting. At Hershey, the same ideas carry over to consumer choice:
discrete, high-dimensional data on what shoppers put in a basket, paired with
tractable optimization for assortment decisions. The domains differ; the
underlying problem, making sense of many interdependent discrete choices, is
the same.

## Where I want to go next

**Decision science for experimentation.** Most A/B testing is still framed as
traditional hypothesis testing, and the modern ML variants mostly answer the
same question: is the effect significant?  I am very interested in exploring
methods that are more aligned with what the executive really wants to know:
*what is the risk of not deploying this?* Two toolkits appear better suited to
answer this question directly.  Bayesian decision theory can be generalized
with the risk associated with the decision space is accurately quantified.
Then the question of statistical signifance shifts to evaluating the the
posterior probability that a feature or strategy delivers incremental lift, and
the expected loss of shipping it versus holding it back. Recent advances in the
field also consider handling many metrics at once, pooling information across
them and shrinking noisy ones instead of leaning on multiple-testing
corrections that are principled, but increase the bar for detecting significant
effects.  Effects sizes are often small, yet practically often very important
(a small .5\% lift can mean millions of dollars), thus methods that are better
attuned to expected loss around the decision space better inform the risk
associated with each decision.  I am also excited about E-values which solve
the monitoring problem: they measure cumulative evidence that stays valid
however often we look, so a test can stop as soon as the answer is clear. The
eliminated risk of peaking at the data invites collaboration as the
statistician is no longer the scold to ensure early peaking doesn't increase
the false discovery rate.  E-values can also be combined across tests while
keeping formal error guarantees.  From exploration of the literature, their
appear to be low hanging fruit in the application of more formal decision
theory to business questions. 

**New problems, approached like research.** As I consider the shape of my
future career, I want to put myself in environments that will spur continued
growth through challenging business problems and growing my technical toolkit. 
My PhD training is less about any one method than about how to take on a problem I
haven't seen before: dig into the literature, understand the limitations,
risks, and tradeoffs between candidate models, and learn new techniques
independently. I pair that with the work of building consensus on what question
we actually need to answer, so the effort goes into the right problem.
