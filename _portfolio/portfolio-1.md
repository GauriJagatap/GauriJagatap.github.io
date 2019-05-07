---
title: "Compressive phase retrieval under image priors"
excerpt: "<br/><img src='/images/pr.png'>"
collection: portfolio
---

<font size="+2"> Abstract </font>

<p style='text-align: justify;'>
We consider the problem of recovering an n-dimensional signal, from m magnitude-only measurements. This is a stylized version of the classical phase retrieval problem, and is a fundamental challenge in nano- and bio-imaging systems, astronomical imaging, and speech processing. It is well known that the above problem is ill-posed, and therefore some additional assumptions on the signal and/or the measurements are necessary.</p>

<p style='text-align: justify;'>
In this paper, we first study the case where the underlying signal x* is s-sparse. For this case, we develop a novel recovery algorithm that we call <i>Compressive Phase Retrieval with Alternating Minimization</i>, or <i>CoPRAM</i>. Our algorithm is simple and be obtained via a natural combination of the classical alternating minimization approach for phase retrieval with the CoSaMP algorithm for sparse recovery. Despite its simplicity, we prove that our algorithm achieves a sample complexity of O(s^2 log n) with Gaussian measurements a_i, which matches the best known existing results; moreover, it also demonstrates linear convergence in theory and practice. An appealing feature of our algorithm is that it requires no extra tuning parameters other than the signal sparsity level s.</p>

<p style='text-align: justify;'>
We then consider the case where the underlying signal x^* arises from <i>structured</i> sparsity models. We specifically examine the case of <i>block-sparse</i> signals with uniform block size of b and block sparsity k=s/b. For this problem, we design a recovery algorithm that we call <i>Block CoPRAM</i> that further reduces the sample complexity to O(ks log n). For sufficiently large block lengths of b=s, this bound equates to O(s log n). Further, we consider power-law decaying sparse signals, further lowering sample complexity to O(s log n). We also present an extention to rooted tree-sparse signals and analyze the descent criterion of the alternating minimization scheme. We find that, as long as a good initialization is provided, the sample complexity of this problem can be brought down to O(s), which is information theoretically optimal. To our knowledge, this constitutes the first end-to-end linearly convergent group of algorithms for phase retrieval where the Gaussian sample complexity has a sub-quadratic dependence on the signal sparsity level. </p>


<font size="+2"> Code </font>

You can also find all codes related to the paper on my <a target="_blank" href='https://github.com/GauriJagatap/model-copram'> GitHub page</a>.

<font size="+2"> Publications </font>

1. **G. Jagatap**, C. Hegde, "Fast, sample efficient algorithms for structured phase retrieval", Advances in Neural Information Processing Systems (NIPS), 2017. (Acceptance rate: 20.93%) [ <a target="_blank" href='http://papers.nips.cc/paper/7077-fast-sample-efficient-algorithms-for-structured-phase-retrieval'>Paper</a> / [Poster]({{ site.url }}/assets/poster.pdf) / <a target="_blank" href='https://github.com/GauriJagatap/model-copram'>Code</a> ]

2. **G. Jagatap**, C. Hegde, "Sample efficient algorithms for recovering structured signals from magnitude-only measurements", IEEE Transactions on Information Theory, 2019. 
[<a target="_blank" href='https://arxiv.org/abs/1705.06412'>arXiv Preprint</a>/ <a target="_blank" href='https://ieeexplore.ieee.org/abstract/document/8660586'>Paper</a> / <a target="_blank" href='https://github.com/GauriJagatap/model-copram'>Code</a>]

3. **G. Jagatap**, C. Hegde, "Towards sample-optimal methods for solving random quadratic equations with structure", IEEE International Symposium on Information Theory (ISIT), [[Preprint]({{ site.url }}/assets/ISIT18.pdf) / <a target="_blank" href='https://ieeexplore.ieee.org/document/8437770'>Paper</a> / [Talk]({{ site.url }}/assets/ISIT18talk.pdf) / <a target="_blank" href='https://github.com/GauriJagatap/model-copram/tree/trees'>Code</a> ], 2018.
