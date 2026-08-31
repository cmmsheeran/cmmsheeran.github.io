---
layout: page
title: research
permalink: /research/
description: Scale, structure, and dynamics in complex systems.
nav: true
nav_order: 1
horizontal: true
---

My work is organized around a central question:

> **How do microscopic interactions generate stable, interpretable, and predictive organization at larger scales?**

I approach this question using tools from network science, statistical physics, stochastic processes, spectral theory, and Bayesian inference. Rather than assuming a useful scale in advance, I ask which collective variables are supported by the underlying structure and dynamics, how robustly they can be inferred, and when they form an autonomous description of the system.

## Mesoscale structure and dynamic readouts

A network does not by itself determine the patterns an observer will see. Mesoscale organization also depends on the dynamics evolving on that network and on the readout used to turn microscopic activity into modules, states, or order parameters. I develop probabilistic and spectral methods for quantifying this dependence, including the expected value, variability, stability, and capacity of coarse-grained observables.

This work is motivated especially by neural systems. A largely fixed connectome must support rapidly changing patterns of coordinated activity; the aim is to determine mathematically which aspects of that changing functional organization follow from anatomy, dynamics, and measurement.

## Coarse-graining and emergence

A useful macroscopic description should do more than compress a system: it should preserve the mechanisms needed to predict its behavior. I study when network dynamics can be reduced to a smaller set of collective variables, how renormalization changes those variables across scales, and how failures of dynamical closure reveal information that cannot be represented at the coarser level.

## Collective inference from networked observations

Pairwise observations—such as wins and losses—form a comparison network rather than a simple ordered list. I develop hierarchical probabilistic models that infer latent skill while accounting for uneven schedules, group structure, uncertainty, and the effective depth of competition. This provides a complementary setting in which global organization must be inferred from sparse, structured local interactions.

## Previous work

My earlier work used spatially embedded recurrent neural networks to study how physical and communication constraints shape learned structure and function. We found that spatial embedding promotes a distinctive low-entropy modular organization while allowing heterogeneous spectral dynamics.

---

## Current projects

<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %}
        {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
</div>
