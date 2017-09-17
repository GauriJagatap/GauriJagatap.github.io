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

<font size="+2"> Project description </font>

<p style='text-align: justify;'>
In our previous work on <a target="_blank" href='https://arxiv.org/abs/1705.06412'> structured phase retrieval</a>, we noted the advantages of incorporating a sparsity constraint in the phase retrieval algorithm (we call our algorithm CoPRAM). The advantages of this are two fold: fewer number of samples are required for efficient recovery and the recovery procedure is also computationally much faster. </p>

<p style='text-align: justify;'>
In this exploratory report, we consider the problem of super-resolution for sub-diffraction imaging. We try to adapt conventional Fourier ptychographic approaches, specifically the one described in <a target="_blank" href='https://arxiv.org/abs/1510.08470'>the reference paper</a> for a subset of problems where the
images to be acquired have an underlying structure. For the purpose of this study, we analyze primarily sparse images. We also extend our study to block sparse images. We find that such sparsity assumptions require fewer samples for the recovery procedure and are more feasible to implement.</p>

<font size="+2"> Simulation results </font>

<p style='text-align: justify;'>
Some results showcasing preliminary advantage that our sparse phase retrieval algorithm offers, over conventional approaches that do not consider any model on the signal/image under consideration: </p>

<div style="text-align: center;">
<img src="{{ site.url }}/assets/images/FP1.JPG"/>
</div>

<div style="text-align: center;">
<img src="{{ site.url }}/assets/images/FP2.JPG" />
</div>

<div style="text-align: center;">
<img src="{{ site.url }}/assets/images/FP3.JPG" />
</div>

<div style="text-align: center;">
<img src="{{ site.url }}/assets/images/FP4.JPG" />
</div>


<div style="text-align: center;">
<img src="{{ site.url }}/assets/images/FP5.JPG" />
</div>

You can find a more detailed report on this project [here]({{ site.url }}/assets/FP_report.pdf).

<font size="+2"> References </font>

[1] "Toward Long Distance, Sub-diffraction Imaging Using Coherent Camera Arrays" 
J. Holloway, M.S. Asif, M.K. Sharma, N. Matsuda, R. Horstmeyer, O. Cossairt, and A. Veeraraghavan
IEEE Transactions on Computational Imaging, 2016.

[2] "Phase Retrieval Using Structured Sparsity: A Sample Efficient Algorithmic Framework." 
G. Jagatap, and C. Hegde
arXiv preprint arXiv:1705.06412 (2017).

New to sub-diffractive imaging? Find some quick info on this <a target="_blank" href='https://docs.google.com/document/d/1Lr3UwDjWWkiqotms7-4pSN835EvrSuKECAPUtXfWmEI/edit?usp=sharing'>cheat sheet.</a>
