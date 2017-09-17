---
title: "Sub-diffractive super-resolution of structured images using Fourier ptychography"
layout: post
date: 2017-09-12 19:59
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- phase retrieval
category: project
mathjax : true
---
<p style='text-align: justify;'>
We extend the work by <a target="_blank" href='https://arxiv.org/abs/1510.08470'>Holloway et. al.</a> for images and videos with inherent structures such as sparsity and low rank. </p>

In our previous work on <a target="_blank" href='https://arxiv.org/abs/1705.06412'> structured phase retrieval</a>, we noted the advantages of incorporating a sparsity constraint in the phase retrieval algorithm (we call our algorithm CoPRAM). The advantages of this are two fold: fewer number of samples are required for efficient recovery and the recovery procedure is also computationally much faster.

In this exploratory report, we consider the problem of super-resolution for sub-diffraction imaging. We try to adapt conventional Fourier ptychographic approaches, specifically the one described in <a target="_blank" href='https://arxiv.org/abs/1510.08470'>the reference paper</a> for a subset of problems where the
images to be acquired have an underlying structure. For the purpose of this study, we analyze primarily sparse images. We also extend our study to block sparse images. We find that such sparsity assumptions require fewer samples for the recovery procedure and are more feasible to implement.

Some results showcasing preliminary advantage that our sparse phase retrieval algorithm offers, over conventional approaches that do not consider any model on the signal/image under consideration:

![Experiment 1.1]({{ site.url }}/assets/images/FP1.JPG)
![Experiment 1.2]({{ site.url }}/assets/images/FP2.JPG)
![Experiment 2.1]({{ site.url }}/assets/images/FP3.JPG)
![Experiment 2.2]({{ site.url }}/assets/images/FP4.JPG)
![Experiment 3.1]({{ site.url }}/assets/images/FP5.JPG)
![Experiment 3.2]({{ site.url }}/assets/images/FP6.JPG)
![Experiment 4.1]({{ site.url }}/assets/images/FP7.JPG)
![Experiment 4.2]({{ site.url }}/assets/images/FP8.JPG)

You can find a more detailed report on this project [here](/assets/FP_report.pdf).

**New to sub-diffractive imaging? Find some quick info on this <a target="_blank" href='https://docs.google.com/document/d/1Lr3UwDjWWkiqotms7-4pSN835EvrSuKECAPUtXfWmEI/edit?usp=sharing'>cheat sheet.</a>

