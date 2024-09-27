---
layout: distill
title: Neuralacoustics
description: A Deep Learning Framework For Musical Acoustics Simulations
img: assets/img/2024-aimc-neuralacoustics.jpg
category: Audio Synthesis
related_publications: true
date: 2024-09-09
featured: true

authors:
  - name: Jiafeng Chen
    affiliations:
      name: University of Michigan
  - name: Kıvanç Tatar
    url: "https://www.kivanctatar.com"
    affiliations: 
      name: Chalmers University of Technology, Sweden
  - name: Victor Zappi
    url: "https://coe.northeastern.edu/people/zappi-victor/"
    affiliations: 
      name: Northeastern University, USA

bibliography: aimc24-2.bib
toc: false
---

## Description

The acoustic modeling of musical instruments is a heavy computational process, often bound to the solution of complex systems of partial differential equations (PDEs). Numerical models can achieve a high level of accuracy, but they may take up to several hours to complete a full simulation, especially in the case of intricate musical mechanisms. The application of deep learning, and in particular of neural operators that learn mappings between function spaces, has the potential to revolutionize how acoustics PDEs are solved and noticeably speed up musical simulations. However, extensive research is necessary to understand the applicability of such operators in musical acoustics; this requires large datasets, capable of exemplifying the relationship between input parameters (excitation) and output solutions (acoustic wave propagation) per each target musical instrument/configuration. With this work <d-cite key="chen_sounding_2024"></d-cite>, we present an open-access, open-source framework designed for the generation of numerical musical acoustics datasets and for the training/benchmarking of acoustics neural operators. We first describe the overall structure of the framework and the proposed data generation workflow. Then, we detail the first numerical models that were ported to the framework. This work is a first step towards the gathering of a research community that focuses on deep learning applied to musical acoustics, and shares workflows and benchmarking tools.

The paper is now accessible via the following link: 
<https://aimc2024.pubpub.org/pub/5cl1cvmy/release/1>

## Code

<i class="fa-brands fa-github"></i> <a>https://github.com/ktatar/neuralacoustics</a>

## Acknowledgements


This work was supported by the Wallenberg AI, Autonomous Systems and Software Program – Humanities and Society (WASP-HS) funded by the Marianne and Marcus Wallenberg Foundation and the Marcus and Amalia Wallenberg Foundation. 
<div>
  <div class="row">
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/wasphs.png" title="wasp-hs logo" %}
      </div>
  </div>
</div>