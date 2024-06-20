---
layout: distill
title: Interfacing ErgoJr with Creative Coding Platforms
description: at ACM Movement Computing Conference 2024
img: assets/img/ergojr.jpg
importance: 1
category: Movement Computing
related_publications: true
date: 2024-05-30
featured: true

authors:
  - name: Matto Caravati
    url: 
    affiliations:
      name: Chalmers University of Technology
  - name: Kıvanç Tatar
    url: "https://www.kivanctatar.com"
    affiliations: 
      name: Chalmers University of Technology

bibliography: moco24.bib
toc: true
---

<div class=".l-body">

{% include figure.liquid loading="eager" path="assets/img/ergojr.jpg" title="ErgoJr" %}

</div>

## Description

Creative coding platforms represent a genre of software that facilitates users in exploring and manifesting their creative inclinations through programming endeavors. Serving as an intermediary between coding practices and artistic expression, these platforms offer simplified coding syntaxes and user-friendly interface libraries.

The focal point of our work lies in the development of a software infrastructure based on a client-server architecture to allow the remote control of a low-cost educational robot such as the Poppy Ergo Jr. The client component is written in C++, featuring bindings to fit diverse platforms such as Pure Data, Processing, P5.js, or Python. The server component, implemented in Python, enables both prototyping and experimentation for users with varying degrees of experience in software programming.

In our design, we opted for the use of the Open Sound Control (OSC) protocol in tandem with UDP, and Websockets in tandem with TCP. This choice allows real-time communication between client and server, as opposed to more conventional protocols like HTTP. While considering alternatives such as WebRTC, we found its implementation complexity and reliance on third-party servers for peer-to-peer connectivity to complexify the process too much.

Communication between the robot and the server was made using a serial connection with an OpenCM9.04 development board flashed with a custom firmware. This board features multiple MOLEX connectors, allowing plug-and-play connectivity with the Poppy Ergo Jr.

Stay tuned for the launch of the ACM Movement and Computing Conference 2024 Proceedings, after which the full paper will be accessible.

## Resources

### Architecture



### Code

<i class="fa-brands fa-github"></i> <a>https://github.com/mcaravati/sp-dr</a>