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

Optimal Experimental Design (OED) under Hyperparameter Uncertainty
------

Building on the previous project, we consider the problem of how to optimally place sensors to maximize information gain in problems with uncertain hyperparameters. In particular, the hyperparameters play an especially significant role in sequential OED problems, in which previous measurements are used to inform later sensor placements, since hyperparameters can be inferred to improve placements. We adapt the D-optimal criterion to take advantage of the efficient evaluation methods developed above to accelerate the computationally intensive optimization loop of OED.

Joint work with [Noemi Petra](https://faculty.ucmerced.edu/npetra/) at UC Merced, and Georg Stadler.

Connecting PDE-governed Inverse Problems to INLA
------

While the inverse problems community has been advancing methods for Bayesian inference problems with hyperparameters, the geostatistics community has developed a widely adopted method, Integrated Nested Laplace Approximations (INLA), which addresses strikingly similar problems. Together with the original author of INLA, we are attempting to bring the two perspectives into a shared framework to illustrate the commonalities and the areas where the methods differ, so that practitioners from both fields can benefit from each other's work, a goal reflected in our upcoming minisymposium at SIAM CSE 27: "Sampling-free Bayesian Inference: Bridging Spatial Statistics and PDE-governed Inverse Problems".

Joint work with [Håvard Rue](https://www.kaust.edu.sa/en/study/faculty/haavard-rue) (developer of INLA) and [Lisa Gaedke-Merzhäuser](https://cemse.kaust.edu.sa/profiles/lisa-gaedke-merzhauser) at KAUST, and with Georg Stadler.




