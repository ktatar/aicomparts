---
layout: distill
title: Raw Music From Free Movements
description: Human Body Pose Sequences into Audio Waveforms.
img: assets/img/ramfem-crop.jpg
importance: 1
category: Audio Synthesis
related_publications: true
date: 2020-10-20
featured: true

authors:
  - name: Kıvanç Tatar
    url: "https://www.kivanctatar.com"
    affiliations:
      name: Chalmers University of Technology
  - name: Daniel Bisig
    url: 
    affiliations: 
      name: Zurich University of the Arts

bibliography: ramfem.bib
toc: true

---
## Description
Raw Music from Free Movements is a deep learning architecture that translates pose sequences into audio waveforms. The architecture combines a sequence-to-sequence model generating audio encodings and an adversarial autoencoder that generates raw audio from audio encodings. Experiments have been conducted with two datasets: a dancer improvising freely to a given music, and music created through simple movement sonification. The paper presents preliminary results. These will hopefully lead closer towards a model which can learn from the creative decisions a dancer makes when translating music into movement and then follow these decisions reversely for the purpose of generating music from movement.
## Architecture

<div class="fake-img l-page-outset">
{% include figure.liquid loading="eager" path="assets/img/ramfem-arch.png" title="The Deep Learning architecture in Raw Music From Free Movements" %}
</div>
<div class="caption">
    The Deep Learning architecture in Raw Music From Free Movements.
</div>

## Examples


Two different datasets were employed for training, named improvisation dataset and sonification dataset. The improvisation dataset consists of pose sequences and audio that have been recorded while a dancer was freely improvising to a given music. The dancer is an expert with a specialisation in contemporary dance and improvisation. The music consists of short excerpts of royalty free music including experimental electronic music, free jazz, and contemporary classic. The pose sequences have been acquired using the markerless motion capture system (The Captury ) in the iLab at MotionBank, University for Applied Research, Mainz. The recording is 10 minutes in length which corresponds to a sequence of 30000 poses. Each pose consists of 29 joints whose relative orientations are represented by quaternions.

The sonification dataset contains the same pose sequences as the improvisation dataset. The audio of this dataset was created afterwards, through sonification, employing a very simple sound synthesis consisting of two sine oscillators controlled by the dancer’s hands. The frequency and amplitude of each oscillator are proportional to the height and velocity of the corresponding hand, respectively. The authors created this dataset to verify the performance of RAMFEM.

## Resources

### Code
<i class="fa-brands fa-github"></i> <a>https://bitbucket.org/dbisig/rawmusicfromfreemovements</a>

### Supplementary Material

<i class="fa-solid fa-plus"></i> <a>https://zenodo.org/record/4656086</a>

## Acknowledgements

This work has been supported by the Swiss National Science Foundation, the Natural Sciences and Engineering Research Council of Canada, and Social Sciences and Humanities Research Council of Canada.

Ce travail est supporté par le Fonds national Suisse de la recherche scientifique, le Conseil national des sciences et de l’ingénieurie du Canada, et le Conseil national des sciences humaines et sociales du Canada.
<div class="fake-img l-page-outset">
  <div class="row">
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/marie-curie.png" title="Marie Curie logo" %}
      </div>
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/icst.png" title="Institute for Computer Music and Sound Technologies at Zurich University of the Arts, Switzerland" %}
      </div>
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/zhdk.png" title="Zurich University of the Arts logo" %}
      </div>
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/icst.png" title="Institute for Computer Music and Sound Technologies at Zurich University of the Arts, Switzerland" %}
      </div>
  </div>
</div>