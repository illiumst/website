---
layout: single
title:  "Voronoi Patches"
categories: research audio deep-learning anomalie-detection 
excerpt: "Evaluating A New Data Augmentation Method"
header:
  teaser: assets/figures/17_vp_teaser.jpg
---

![Organism Network Architecture](\assets\figures\17_vp_lion.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

Overfitting is a problem in Convolutional Neural Networks (CNN) that causes poor generalization of models on unseen data. To remediate this problem, many new and diverse data augmentation methods (DA) have been proposed to supplement or generate more training data, and thereby increase its quality. In this work, we propose a new data augmentation algorithm: VoronoiPatches (VP). We primarily utilize non-linear recombination of information within an image, fragmenting and occluding small information patches. Unlike other DA methods, VP uses small convex polygon-shaped patches in a random layout to transport information around within an image. Sudden transitions created between patches and the original image can, optionally, be smoothed. In our experiments, VP outperformed current DA methods regarding model variance and overfitting tendencies. We demonstrate data augmentation utilizing non-linear re-combination of information within images, and non-orthogonal shapes and structures improves CNN model robustness on unseen data.
{% cite illium2022voronoipatches %}

:trophy: This paper won the conference's [Best Poster Award](https://icaart.scitevents.org/PreviousAwards.aspx?y=2024#2023), which is a special honor. :trophy:

![Dropout](\assets\figures\17_vp_results.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
