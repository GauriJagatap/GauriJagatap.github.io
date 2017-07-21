---
title: "Phase retrieval of structured signals"
layout: post
date: 2017-03-12 19:48
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- machine learning
- data science
category: project
mathjax : true
---

We consider the problem of recovering a signal $\mathbf{x}^* \in \mathbb{R}^n$, from magnitude-only measurements, $y_i = \| \left\langle {\mathbf{a}_i},{\mathbf{x}^*} \right\rangle \| $ for $i=\{1,2,\ldots,m\}$. This is a stylized version of the classical \emph{phase retrieval problem}, and is a fundamental challenge in nano- and bio-imaging systems, astronomical imaging, and speech processing. It is well known that the above problem is ill-posed, and therefore some additional assumptions on the signal and/or the measurements are necessary.

In this paper, we first study the case where the underlying signal $\mathbf{x}^*$ is $s$-sparse. For this case, we develop a novel recovery algorithm that we call \emph{Compressive Phase Retrieval with Alternating Minimization}, or \emph{CoPRAM}. Our algorithm is simple and be obtained via a natural combination of the classical alternating minimization approach for phase retrieval with the CoSaMP algorithm for sparse recovery. Despite its simplicity, we prove that our algorithm achieves a sample complexity of $O(s^2 \log n)$ with Gaussian measurements $\mathbf{a}_i$, which matches the best known existing results; moreover, it also demonstrates linear convergence in theory and practice. An appealing feature of our algorithm is that it requires no extra tuning parameters other than the signal sparsity level $s$.

We then consider the case where the underlying signal $\mathbf{x}^*$ arises from \emph{structured} sparsity models. We specifically examine the case of \emph{block-sparse} signals with uniform block size of $b$ and block sparsity $k=s/b$. For this problem, we design a recovery algorithm that we call \emph{Block CoPRAM} that further reduces the sample complexity to $O{ks \log n}$. For sufficiently large block lengths of $b=\Theta(s)$, this bound equates to $O(s \log n)$. To our knowledge, this constitutes the first end-to-end linearly convergent algorithm for phase retrieval where the Gaussian sample complexity has a sub-quadratic dependence on the signal sparsity level.

You can read the full paper on <a target="_blank" href='https://arxiv.org/abs/1705.06412'> arXiv </a>.

You can also find all codes related to the paper on my <a target="_blank" href='https://github.com/GauriJagatap/model-copram'> GitHub page </a>.