---
layout: distill
title: Raw Music From Free Movements
description: Human Body Pose Sequences into Audio Waveforms.
img: assets/img/publication_preview/ramfem-crop.jpg
importance: 2
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
Raw Music from Free Movements<d-cite key="bisig_raw_2021"></d-cite> is a deep learning architecture that translates pose sequences into audio waveforms. The architecture combines a sequence-to-sequence model generating audio encodings and an adversarial autoencoder that generates raw audio from audio encodings. Experiments have been conducted with two datasets: a dancer improvising freely to a given music, and music created through simple movement sonification. The paper presents preliminary results. These will hopefully lead closer towards a model which can learn from the creative decisions a dancer makes when translating music into movement and then follow these decisions reversely for the purpose of generating music from movement.
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

The authors’ thanks go to the dancers who have contributed countless hours o their spare time to the motion capture recordings. Further thanks go to MotionBank for providing their infrastructure and assisting in the recordings. This research is conducted in the context of a Marie Curie Fellowship and is funded by the European Union. The collaboration of the second author has been supported by the Canada Council for the Arts.'

<div>
  <div class="row">
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/marie-curie.png" title="Marie Curie logo" %}
      </div>
      <div class="col-sm mt-3 mt-md-0">
          {% include figure.liquid loading="eager" path="assets/img/logos/cca.png" title="Canada Council for the Arts" %}
      </div>
  </div>
</div>