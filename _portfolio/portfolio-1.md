---
title: "Inverse Imaging with Deep Untrained Neural Network Priors"
excerpt: "<br/><img src='/images/NetPGD.png'>"
collection: portfolio
---

<font size="+2"> Project description </font>

Deep neural networks as image priors have been recently introduced for problems such as denoising, super-resolution and inpainting with promising performance gains over hand-crafted image priors such as sparsity and low-rank. Unlike learned generative priors they do not require any training over large datasets. However, few theoretical guarantees exist in the scope of using untrained network priors for inverse imaging problems. We explore new applications and theory for untrained network priors. Specifically, we consider the problem of solving linear inverse problems, such as compressive sensing, as well as non-linear problems, such as compressive phase retrieval. We model images to lie in the range of an untrained deep generative network with a fixed seed. We further present a projected gradient descent scheme that can be used for both compressive sensing and phase retrieval and provide rigorous theoretical guarantees for its convergence. We also show both theoretically as well as empirically that with deep network priors, one can achieve better compression rates for the same image quality compared to hand crafted priors. We also extend the application of deep image priors to HDR imaging.

<font size="+2"> Code </font>

You can find all codes related to the paper on my <a target="_blank" href='https://github.com/GauriJagatap/invimaging-deeppriors'> GitHub page</a>.

<font size="+2"> Papers: </font>

1. **G. Jagatap**, C. Hegde, "Algorithmic Guarantees for Inverse Imaging with Untrained Network Priors", Advances in Neural Information Processing Systems, 2019. (Acceptance rate: 21.18%)  [<a target="_blank" href='https://arxiv.org/abs/1906.08763'> Preprint </a> / <a target="_blank" href='https://github.com/GauriJagatap/invimaging-deeppriors'> Code </a>]

2. **G. Jagatap**, C. Hegde, "Phase Retrieval using Untrained Neural Network Priors", NeurIPS Workshop on Solving Inverse Problems with Deep Learning, 2019. [ <a target="_blank" href= 'https://openreview.net/forum?id=ryl7QwPEIr'>Paper</a> ]

3. **G. Jagatap**, C. Hegde, "High dynamic range imaging using deep image priors", 2019. [[Preprint]({{ site.url }}/assets/hdrimage.pdf)]
