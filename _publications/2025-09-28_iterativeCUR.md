---
title: "Fast Rank Adaptive CUR via a Recycled Small Sketch"
collection: publications
permalink: /publications/2025-09-28_iterativeCUR
excerpt: 
date: 2025-09-26
venue: 
paperurl: 
preprinturl: https://arxiv.org/abs/2509.21963 
citation: 'Pritchard, N., Park, T., Nakasukasa, Y., & Martinsson, G. (2025). Fast Rank Adaptive CUR via a Recycled Small Sketch. arXiv preprint arXiv:2509.21963.'
note: 
---
<b> Abstract </b>:
The computation of accurate low-rank matrix approximations is central to improving the scalability of various techniques in machine learning, uncertainty quantification, and control. Traditionally, low-rank approximations are constructed using SVD-based approaches such as truncated SVD or RandomizedSVD. Although these SVD approaches -- especially RandomizedSVD -- have proven to be very computationally efficient, other low-rank approximation methods can offer even greater performance. One such approach is the CUR decomposition, which forms a low-rank approximation using direct row and column subsets of a matrix. Because CUR uses direct matrix subsets, it is also often better able to preserve native matrix structures like sparsity or non-negativity than SVD-based approaches and can facilitate data interpretation in many contexts. This paper introduces IterativeCUR, which draws on previous work in randomized numerical linear algebra to build a new algorithm that is highly competitive compared to prior work: (1) It is adaptive in the sense that it takes as an input parameter the desired tolerance, rather than an a priori guess of the numerical rank. (2) It typically runs significantly faster than both existing CUR algorithms and techniques such as RandomizedSVD, in particular when these methods are run in an adaptive rank mode. Its asymptotic complexity is O(mn+(m+n)r2+r3) for an m×n matrix of numerical rank r. (3) It relies on a single small sketch from the matrix that is successively downdated as the algorithm proceeds. We demonstrate through extensive experiments that IterativeCUR achieves up to 4× speed-up over state-of-the-art pivoting-on-sketch approaches with no loss of accuracy, and up to 40× speed-up over rank-adaptive randomized SVD approaches.
---
