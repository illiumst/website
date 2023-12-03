---
layout: single
title:  "Point Cloud Segmentation"
categories: research 
excerpt: "Segmetation of point clouds into primitive building blocks."
header:
  teaser: assets/figures/4_point_cloud_segmentation_teaser.jpg
---

![Point Cloud Segmentation](\assets\figures\4_point_cloud_pipeline.jpg){:style="display:block; margin-left:auto; margin-right:auto;"}

The segmentation and fitting of solid primitives to 3D point clouds is a complex task. Existing systems are restricted either in the number of input points or the supported primitive types. This paper proposes a hybrid pipeline that is able to reconstruct spheres, bounded cylinders and rectangular cuboids on large point sets. It uses a combination of deep learning and classical RANSAC for primitive fitting, a DBSCAN-based clustering scheme for increased stability and a specialized Genetic Algorithm for robust cuboid extraction. In a detailed evaluation, its performance metrics are discussed and resulting solid primitive sets are visualized. The paper concludes with a discussion of the approach’s limitations.
{% cite friedrich2020hybrid %}

![Point Cloud Segmentation](\assets\figures\4_point_cloud_segmentation.jpg){:style="display:block; margin-left:auto; margin-right:auto;"}
