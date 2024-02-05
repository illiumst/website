---
layout: single
title:  "Voronoi Patches"
categories: research audio deep-learning anomalie-detection 
excerpt: "Evaluating A New Data Augmentation Method"
header:
  teaser: assets/figures/17_vp_teaser.jpg
---

![Organism Network Architecture](\assets\figures\17_vp_lion.jpg){:style="display:block; width:85%" .align-center}

This study introduces VoronoiPatches (VP), a novel data augmentation algorithm that enhances Convolutional Neural Networks' performance by using non-linear recombination of image information. VP distinguishes itself by utilizing small, convex polygon-shaped patches in random layouts to redistribute information within an image, potentially smoothing transitions between patches and the original image. This method has shown to outperform existing data augmentation techniques in reducing model variance and overfitting, thus improving the robustness of CNN models on unseen data. {% cite illium2022voronoipatches %}

:trophy: Our work was awarded the [Best Poster Award](https://icaart.scitevents.org/PreviousAwards.aspx?y=2024#2023) at ICAART 2023 :trophy:

![Dropout](\assets\figures\17_vp_results.jpg){:style="display:block; width:90%" .align-center}
