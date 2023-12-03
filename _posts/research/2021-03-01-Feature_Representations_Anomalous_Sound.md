---
layout: single
title:  "Anomalous Sound Detection"
categories: research audio deep-learning anomalie-detection
excerpt: "Analysis of Feature Representations for Anomalous Sound Detection"
header:
  teaser: assets/figures/8_anomalous_sound_teaser.jpg
---

![Pipeline](\assets\figures\8_anomalous_sound_features.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

The problem of Constructive Solid Geometry (CSG) tree reconstruction from 3D point clouds or 3D triangle meshes is hard to solve. At first, the input data set (point cloud, triangle soup or triangle mesh) has to be segmented and geometric primitives (spheres, cylinders, ...) have to be fitted to each subset. Then, the size- and shape optimal CSG tree has to be extracted. We propose a pipeline for CSG reconstruction consisting of multiple stages: A primitive extraction step, which uses deep learning for primitive detection, a clustered variant of RANSAC for parameter fitting, and a Genetic Algorithm (GA) for convex polytope generation. It directly transforms 3D point clouds or triangle meshes into solid primitives. The filtered primitive set is then used as input for a GA-based CSG extraction stage. We evaluate two different CSG extraction methodologies and furthermore compare our pipeline to current state-of-the-art methods.
{% cite muller2020analysis %}
