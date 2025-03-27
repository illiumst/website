---
layout: single
title: "3D Primitive Segmentation"
categories: research
tags: computer-vision 3d-processing point-clouds segmentation deep-learning genetic-algorithms
excerpt: "Hybrid method segments/fits primitives in large 3D point clouds."
header:
  teaser: /assets/figures/4_point_cloud_segmentation_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

<center>
  <img src="/assets/figures/4_point_cloud_pipeline.jpg" alt="Diagram illustrating the hybrid point cloud segmentation pipeline" style="display:block; width:100%">
  <figcaption>Overview of the hybrid segmentation and primitive fitting pipeline.</figcaption>
</center><br>

This research addresses challenges in accurately segmenting large-scale 3D point clouds into meaningful geometric primitives, specifically spheres, cylinders, and cuboids. Existing methods often struggle with scalability or robustness when faced with diverse shapes and noisy real-world data.

We propose a novel **hybrid approach** that synergistically combines multiple techniques to overcome these limitations:

1.  **Deep Learning Integration:** Utilized to potentially enhance initial feature extraction or provide guidance for subsequent steps (the exact role should be clarified based on the paper, e.g., pre-segmentation, feature learning).
2.  **RANSAC-based Primitive Fitting:** Employs the robust RANSAC algorithm for accurately fitting simpler geometric shapes like spheres and cylinders to subsets of the point cloud.
3.  **DBSCAN Clustering:** Applied for grouping remaining points or refining segmentation boundaries, effectively handling noise and varying point densities.
4.  **Specialized Genetic Algorithm:** A custom Genetic Algorithm is introduced specifically for the robust detection and fitting of cuboid primitives, which are often challenging for standard fitting methods.

This integrated pipeline demonstrates enhanced stability and robustness compared to methods relying on a single technique. It particularly excels in reconstructing the target primitives from large and complex point sets. The effectiveness of the approach is validated through quantitative performance metrics and qualitative visualizations, with a discussion acknowledging the method's scope and potential limitations. For a detailed technical description and evaluation, please refer to the publication by {% cite friedrich2020hybrid %}.

<center>
  <img src="/assets/figures/4_point_cloud_segmentation.jpg" alt="Example result showing a point cloud segmented into different colored geometric primitives" style="display:block; width:890%">
  <figcaption>Example segmentation result demonstrating primitive identification.</figcaption>
</center>