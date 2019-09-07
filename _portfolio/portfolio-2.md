---
title: "Provable algorithms for machine learning"
excerpt: "<br/><img src='/images/resnet.png'>"
collection: portfolio
---

<font size="+2"> Project description </font>

We propose and analyze algorithms for training ReLU networks with skipped connections. Skipped connections
are the key feature of residual networks (or ResNets) which have been shown to provide superior performance in deep learning applications. We analyze two approaches for training such networks, gradient descent and alternating minimization, and compare convergence criteria of both methods. We show that under typical (Gaussianity) assumptions on the ddimensional input data, both gradient descent and alternating
minimization provably converge in a linearly convergent fashion, assuming any good enough initialization; moreover, we show that a simple "identity" initialization suffices. Furthermore, we provide statistical upper bounds which indicate that n = O(d^3) suffice to achieve this convergence rate. To our knowledge, these
constitute the first global parameter recovery guarantees for shallow ResNet-type networks with ReLU activations.

<font size="+2"> Code </font>

You can find all codes related to the paper on my <a target="_blank" href='https://github.com/GauriJagatap/altminrelu'> GitHub page</a>.

<font size="+2"> Publications </font>

1. **G. Jagatap**, C. Hegde, "Linearly Convergent Algorithms for Learning Shallow Residual Networks. ", IEEE International Symposium on Information Theory (ISIT), 2019. [[Preprint]({{ site.url }}/assets/ISIT19.pdf)]

