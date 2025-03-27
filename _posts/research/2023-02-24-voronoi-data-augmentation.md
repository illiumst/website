---
layout: single
title: "Voronoi Data Augmentation"
categories: research
tags: data-augmentation computer-vision deep-learning convolutional-neural-networks
excerpt: "VoronoiPatches improves CNN robustness via non-linear recombination augmentation."
header:
  teaser: /assets/figures/17_vp_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

Data augmentation is essential for improving the performance and generalization of Convolutional Neural Networks (CNNs), especially when training data is limited. This research introduces **VoronoiPatches (VP)**, a novel data augmentation algorithm based on the principle of **non-linear recombination** of image information.

<center>
  <img src="/assets/figures/17_vp_lion.jpg" alt="Example of an image augmented with VoronoiPatches, showing polygon patches blended onto a lion image" style="display:block; width:85%">
  <figcaption>Visual example of the VoronoiPatches augmentation applied to an image.</figcaption>
</center><br>

Unlike traditional methods that often apply uniform transformations or cutout regions, VP operates by:
1.  Generating a random layout of points within an image.
2.  Creating a Voronoi diagram based on these points, partitioning the image into unique, convex polygon-shaped patches.
3.  Redistributing information between these patches or blending information across patch boundaries (specific mechanism detailed in the paper).

This approach potentially allows for smoother transitions between augmented regions and the original image compared to sharp cutout methods. The core idea is to encourage the CNN to learn more robust features by exposing it to varied, non-linearly recombined versions of the input data.

---

<div style="text-align: center; margin: 1em 0; font-weight: bold; color: #D4AF37;">
:trophy: Best Poster Award - ICAART 2023 :trophy:<br>
<small>(<a href="https://icaart.scitevents.org/PreviousAwards.aspx?y=2024#2023" target="_blank" rel="noopener noreferrer">Official Link</a>)</small>
</div>

---

Evaluations demonstrate that VoronoiPatches can effectively **reduce model variance and combat overfitting**. Comparative studies indicate that VP **outperforms several existing state-of-the-art data augmentation techniques** in improving the robustness and generalization performance of CNN models on unseen data across various benchmarks. {% cite illium2023voronoipatches %}

<center>
  <img src="/assets/figures/17_vp_results.jpg" alt="Graphs showing performance comparison (e.g., accuracy, loss) of VoronoiPatches against other augmentation methods" style="display:block; width:90%">
  <figcaption>Comparative results illustrating the performance benefits of VoronoiPatches.</figcaption>
</center><br>