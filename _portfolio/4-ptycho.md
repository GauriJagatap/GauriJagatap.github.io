---
title: "Fourier ptychography for super-resolution under image priors"
excerpt: "<br/><img src='/images/copram.png'>"
collection: portfolio
---


<font size="+2"> Project description </font>

<p style='text-align: justify;'>
In our previous work on <a target="_blank" href='https://arxiv.org/abs/1705.06412'></a> structured phase retrieval, we noted the advantages of incorporating a sparsity constraint in the phase retrieval algorithm (we call our algorithm CoPRAM). The advantages of this are two fold: fewer number of samples are required for efficient recovery and the recovery procedure is also computationally much faster. </p>

<p style='text-align: justify;'>
In this exploratory report, we consider the problem of super-resolution for sub-diffraction imaging. We adapt conventional Fourier ptychographic approaches, for a subset of problems where the images to be acquired have an underlying structure. For the purpose of this study, we analyze primarily sparse images. We also extend our study to block sparse images. We find that such sparsity assumptions require fewer samples for the recovery procedure and are more feasible to implement. We also report similar benefits for videos with approximate low-rank structure.</p>

<div style="text-align: center;">
<img src="{{ site.url }}/images/copram.png"/>
</div>

<font size="+2"> Code </font>

You can find the code <a target="_blank" href='https://github.com/GauriJagatap/copram-for-ptycho'>here</a>.

<font size="+2"> Publications </font>

1. **G. Jagatap**, Z. Chen, C. Hegde, N. Vaswani, "Sub-diffraction imaging using Fourier ptychography
and structured sparsity", IEEE International Conference on Acoustics, Speech, and Signal Processing (ICASSP), (Oral Presentation) 2018. [ [Preprint]({{ site.url }}/assets/SFP.pdf) / <a target="_blank" href='https://ieeexplore.ieee.org/document/8461302'>Paper</a> / [Talk]({{ site.url }}/assets/ICASSP18talk.pdf) / <a target="_blank" href='https://github.com/GauriJagatap/copram-for-ptycho'>Code</a> ]

2. Z. Chen, **G. Jagatap**, S. Nayer, C. Hegde, N. Vaswani, "Low rank Fourier ptychography", IEEE International Conference on Acoustics, Speech, and Signal Processing (ICASSP), 2018. [[Preprint]({{ site.url }}/assets/LRFP.pdf) / <a target="_blank" href='https://ieeexplore.ieee.org/document/8462480'>Paper</a> / [Poster]({{ site.url }}/assets/ICASSP18poster.pdf)]

3. **G. Jagatap**, Z. Chen, C. Hegde, N. Vaswani, "Model corrected low rank ptychography",  IEEE International Conference on Image Processing (ICIP), [[Preprint]({{ site.url }}/assets/ICIP18.pdf) / <a target="_blank" href='https://ieeexplore.ieee.org/document/8451403'>Paper</a> / [Poster]({{ site.url }}/assets/ICIP18poster.pdf)], 2018.


4. **G. Jagatap**, Z. Chen, C. Hegde, N. Vaswani, "Efficient Fourier ptychography on structured data: low-rank and sparse models",  IEEE Transactions on Computational Imaging, 2019. [ [Preprint]({{ site.url }}/assets/TCI19.pdf) / <a target="_blank" href='https://github.com/GauriJagatap/copram-for-ptycho'>Code</a> ]

New to sub-diffractive imaging? Find some quick info on this <a target="_blank" href='https://docs.google.com/document/d/1Lr3UwDjWWkiqotms7-4pSN835EvrSuKECAPUtXfWmEI/edit?usp=sharing'>cheat sheet.</a>
