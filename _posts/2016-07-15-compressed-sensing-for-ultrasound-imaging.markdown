---
title: "Compressed sensing for ultrasound imaging"
layout: post
date: 2016-07-15 19:48
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- compressed sensing
- ultrasound imaging
category: project
mathjax : true
---

My introduction to data science and the field of compressed sensing was primarily through the project that I did at the Spectrum Lab of the Indian Institute of Science. It involved analyzing ultrasound images and their underlying sparsity and using the compressed sensing framework to reduce the number of samples acquired in the imaging process. While most ultrasound images are sparse in the standard basis itself, I considered a number of wavelet bases that could emulate the impulse response of the ultrasound transducer, which promotes further sparsity.

It essentially boils down to solving the well known Lasso problem, which I did, using Alternating Directions Method of Multipliers (ADMM).

Lasso Problem.

Link to basic code (on GitHub).

[to be updated]
