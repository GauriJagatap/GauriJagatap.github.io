---
title: "Sparse phase retrieval library"
layout: post
date: 2017-12-19 14:23
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- phase retrieval
- data science
category: blog
mathjax : true
---
<p style='text-align: justify;'>
If you're new to the field of phase retrieval and want to explore some of the techniques that utilize sparsity, I have created a database of algorithms for sparse phase retrieval.

You can find the MATLAB codes for this problem in my <a target="_blank" href='https://github.com/GauriJagatap/model-copram'> GitHub repository for CoPRAM</a>, with all details on the implementation.

The papers in this implementation utilize Gaussian measurements to recover sparse signals from phaseless measurements:
</p>

1. <a target="_blank" href='http://papers.nips.cc/paper/7077-fast-sample-efficient-algorithms-for-structured-phase-retrieval'>CoPRAM</a>
2. <a target="_blank" href='https://papers.nips.cc/paper/5041-phase-retrieval-using-alternating-minimization.pdf'>AltMinSparse</a>
3. <a target="_blank" href='https://arxiv.org/abs/1506.03382'>Thresholded Wirtinger Flow</a>
4. <a target="_blank" href='https://arxiv.org/abs/1611.07641'>SPArse truncated Amplitude flow (SPARTA)</a>

<p style='text-align: justify;'>
Apart from Gaussian measurements, several papers analyze the sparse phase retrieval problem under the Fourier/Short Time Fourier measurement framework. Some papers that explore this option, with publicly available code:
</p>

1. <a target="_blank" href='http://webee.technion.ac.il/people/YoninaEldar/software_det11.php'>GESPAR</a>
2. <a target="_blank" href='https://bitbucket.org/charms/sparsepr'>Robust Sparse phase retrieval made easy</a>

General optimization tools:

<a target="_blank" href='http://webee.technion.ac.il/people/YoninaEldar/software_det12.php'>Sparsity Constrained Nonlinear Optimization: Optimality Conditions and Algorithms</a>


[to be updated]
