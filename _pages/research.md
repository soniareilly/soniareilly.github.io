---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

Marginalization of Hyperparameters in Bayesian Inverse Problems
------

In joint work with my advisor Georg Stadler, I developed fast methods of marginalizing unknown hyperparameters in linear Gaussian PDE-governed Bayesian inverse problems (BIPs). The task in these problems is to recover an underlying parameter of a scientific system from noisy data using Bayesian inference. However, Bayesian inference requires a choice of prior, even when little is known in advance about the parameter. Introducing hyperparameters generalizes the choice of prior, and other features of the problem, while retaining a conditionally Gaussian structure that allows for straightforward evaluation of the posterior.

The difficulty lies in marginalizing out the hyperparameters to recover a distribution over just the parameter of interest, which involves repeated evaluations of the hyperparameter marginal density. For problems with very high dimensional parameters and expensive PDE forward maps, direct methods are computationally prohibitive, and various approximations must be applied. Our methods extend a low-rank approximation framework that is state-of-the-art for problems without hyperparameters to the hyperparameter setting, enabling the cost of a single approximation to be amortized over all evaluations.

For more information, see the [arxiv preprint](https://arxiv.org/abs/2607.03355) or these [slides](/files/SIAM_AN_26_slides.pdf) from July 2026.




