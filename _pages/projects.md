---
permalink: /projects/
title: "Additional Projects"
author_profile: true
redirect_from: 
  - /markdown/
  - /md
  - /markdown.html
---

## Classification between natural and CGI images via Residual CNNs using Sensor Pattern Noise

This was a course project from a course on Digital Image Forensics in Spring 2019 which involved designing an efficient neural network for classifying between natural images and photo-realistic CGI images. The distinguishing feature between natural images obtained via camera, and computer generated images, is that cameras have sensor pattern noise. This can be used as a major discriminative feature, while training a neural network for classifying between these two classes. Additionally, residual networks have shown improved classification performance as compared to vanila CNNs. The objective of this project was to leverage these two factors to detect if a given image is CGI or not. 

You can find details of my project work [here]({{ site.url }}/assets/CGI.pdf)

## Topic extraction via NMF and Sparse PCA

<p style='text-align: justify;'>
I happened to do two course projects in Spring 2017 on two allied problems: (i) Non-negative matrix factorization and (ii) Sparse PCA. While the problem formulation is different, both of them can be used in the context of extracting topics from a given database of documents.</p>

<p style='text-align: justify;'>
In the following slides, I study and demonstrate some results in topic extraction and other applications using both of these formulations. </p>

1. [Non-negative Matrix Factorization](/assets/NMF.pdf)
* Methods used: <a target="_blank" href='http://ieeexplore.ieee.org/document/6166359/'>Nesterov's Orthogonal Gradient Method</a>, <a target="_blank" href='https://arxiv.org/pdf/1208.1237.pdf'>Separable NMF</a>

2. [Sparse PCA]({{ site.url }}/assets/SPCA.pdf)
* Methods used: <a target="_blank" href='http://www.jmlr.org/papers/volume14/yuan13a/yuan13a.pdf'>Truncated Power Method</a>, <a target="_blank" href='https://arxiv.org/abs/1012.0774'>Inverse Power Method</a>.

## Video segmentation under compressive measurements

<p style='text-align: justify;'>
This was my starter kit to the world of data science. I did this project in a largely unguided fashion, but it gave me a good idea about low-rank and sparse problems in signal processing.</p>

An excerpt:

<p style='text-align: justify;'>
Video data transmitted by surveillance cameras is generally processed to detect
moving objects automatically. The video generally consists of a moving object that covers a small fraction of a video frame and majority of the frame is spanned by the background. An intuitive method to separate out the background is by using the fact that the background is stationary, and forms the low rank part of the video volume. On the other hand, the moving objects constitute the sparse component. This decomposition is done using a low rank and sparse decomposition of the video volume.</p>

<p style='text-align: justify;'>
The speed of this processing however, is slowed down by the abundance of data collected, which mostly consists of spells of inactivity. Compressive sensing is a technique used to acquire video data in a different basis, instead of the usual spatial basis, like Fourier or Wavelet, that involves acquiring a small fraction (up to 50% in this project; lower fractions can be used for larger number of frames or higher resolution data) of the data that would have been acquired in the spatial basis.</p>

<p style='text-align: justify;'>
Compressive sensing works when the video data has a low rank and sparse decomposition in some basis, which validates the low sampling rate (less than Nyquist). </p>

The implementation described is based on <a target="_blank" href='https://arxiv.org/abs/1302.1942'> this paper </a>. 

You can find details of my project work [here]({{ site.url }}/assets/vid_seg.pdf). 


