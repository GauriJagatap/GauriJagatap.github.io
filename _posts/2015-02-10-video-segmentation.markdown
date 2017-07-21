---
title: "Video segmentation using ADMM"
layout: post
date: 2015-02-10 19:48
# image: /assets/images/machinelearning.jpg
# headerImage: true
tag:
- machine learning
- data science
category: blog
mathjax : true
---

This was my starter kit to the world of data science. 

Video data transmitted by surveillance cameras is generally processed to detect
moving objects automatically. The video generally consists of a moving object that covers a small fraction of a video frame and majority of the frame is spanned by the background. If each frame is vectorized, and these vectors are concatenated, it is referred to this as the video volume. The video volume can be split into the background and the moving objects (background separation). An intuitive method to separate out the background is by using the fact that the background being stationary, will form the low rank part of the video volume. On the other hand, the moving objects constitute the sparse component. This decomposition is done using a low rank and sparse decomposition of the video volume.

The speed of this processing however, is slowed down by the abundance of data
collected, which mostly consists of spells of inactivity. Compressive sensing is a technique used to acquire video data in a different basis, instead of the usual spatial basis, like Fourier or Wavelet, that involves acquiring a small fraction (up to 50% in this paper, lower fractions can be used for larger number of frames or higher resolution data) of the data that would have been acquired in the spatial basis.

This method works when the given data is sparse in this basis, which validates the low sampling rate (less than Nyquist). Sparse signal recovery from such compressive measurements is a process of minimizing the nuclear norm or l0 norm of the signal (in this case, video volume) in the transformed basis (which ensures sparsity in the transformed basis). The whole video volume can be recovered from this norm minimization and further background separation techniques can be employed to separate out the moving objects.

However, one can formulate the minimization problem such that the background
and moving objects are separated out during the recovery. Moreover, one
1
can choose tight wavelet transforms, which have specific properties that help simplify the minimization problem significantly.

The implementation described is based on <a target="_blank" href='https://arxiv.org/abs/1302.1942'> this paper </a>  >. 

You can find details of my project work [here]({{ site.url }}/assets/vid_seg.pdf). 