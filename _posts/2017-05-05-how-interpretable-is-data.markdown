---
title: "How interpretable is data?"
layout: post
date: 2017-05-05 19:48
image: /assets/images/markdown.jpg
headerImage: false
tag:
- machine learning
- data science
category: blog
author: gaurijagatap
description: Markdown summary with different options
# jemoji: '<img class="emoji" title=":ramen:" alt=":ramen:" src="https://assets.github.com/images/icons/emoji/unicode/1f35c.png" height="20" width="20" align="absmiddle">'
---

## Post content:
I am finally done with my second semester towards my PhD, which means it's time for sum-mer and some-more (or a-lot-more) research!

I happened to have two course projects that I only recently wrapped up, and they turned out to be somewhat related! The two topics being sparse principal component analysis (SPCA) and non-negative matrix factorization (NMF). Both of them, key tools to help <em>interpret </em>data better.

So wait. Given a set of data points, can't we as humans do the intelligible task of interpretation? What do these data-interpretations tools do that we can't?

The answer: they don't do anything we can't. They are just better at interpreting a <em>larger scale</em> of data. They're like a self-organizing library. The librarian no longer has to assign books to particular sections, the books do that themselves (not that we want to put librarians out of business)!

Those familiar with machine learning will automatically recognize this problem formulation as that of <em>unsupervised learning. </em>Employ algorithms that make sense out of data! Principal component analysis, does just that. It tries to represent the variation in the data in descending order. The first principal direction has the maximum variation in data. Usually the first few principal components (usually, this number is $latex \leq r$, where $latex r$ is <em>rank</em> of the data matrix) are sufficient to explain most of the (variation in) data. Now these "directions" are composed of the relative "importance" of its constituent features.

Mathematically speaking, the PCA problem boils down to the singular value decomposition,

$latex M_{d\times n} = (U\Sigma)_{d\times r} V^T_{r \times n}$

where our data matrix $latex M$ is assumed to lie in a lower dimensional subspace of rank $latex r$. Sparse PCA, additionally assumes that the right singular vectors, which are columns of $latex V$ are<em> sparse. </em>

The non-negative matrix factorization problem is similar. A non-negative matrix can be decomposed into non-negative matrices $latex W,H$,

$latex M_{d\times n} = W_{d\times r} H_{r \times n}$

The basic concept utilized in both of these methods is the same: most data has an underlying structure. Imposing the knowledge of this structure should help us extract meaningful information about this data.

Like what? For example in a text dataset, most articles focus on a few core topics. Further, these core topics, can be represented using few core words. This spurred several cool applications, such as detection of <em>trends</em> on social media. In image processing, this has useful applications in <em>segmentation. </em>Representing images as a sum or weighted sum of components. Demixing of audio signals. The list goes on and on and I bet you can already sense the theme in this one.

<img class=" size-full wp-image-779 aligncenter" src="https://thecognitivevortex.files.wordpress.com/2017/05/image02.gif" alt="image02" width="900" height="281" />
I am finally done with my second semester towards my PhD, which means it’s time for sum-mer and some-more (or a-lot-more) research!

