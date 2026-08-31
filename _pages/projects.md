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

> **What is SCALE?**

## Mesoscale structure

A network does not by itself determine the patterns an observer will see. Mesoscale organization also depends on the dynamics evolving on that network and on the readout used to turn microscopic activity into modules, states, or order parameters. I develop probabilistic and spectral methods for quantifying this dependence, including the expected value, variability, stability, and capacity of coarse-grained observables.

This work is motivated especially by neural systems. A largely fixed connectome must support rapidly changing patterns of coordinated activity; the aim is to determine mathematically which aspects of that changing functional organization follow from anatomy, dynamics, and measurement.

### Applications to Neuroscience

This is my most neuro-focused project.

## Coarse-graining and emergence

A generalisable and non-metric network renormalisation using message passing. Closure defects and the mechanisms behind emergent phenomena.  

## Depth in Ranking Models 

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
