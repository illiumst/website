---
layout: single
title:  "Point Cloud Segmentation"
categories: research 
excerpt: "Segmetation of point clouds into primitive building blocks."
header:
  teaser: assets/figures/4_point_cloud_segmentation_teaser.jpg
---

![Point Cloud Segmentation](\assets\figures\4_point_cloud_pipeline.jpg){:style="display:block; width:100%" .align-center}

This paper introduces a hybrid approach for segmenting and fitting solid primitives to 3D point clouds, overcoming limitations in handling large datasets and diverse primitive shapes. By integrating deep learning with RANSAC for primitive fitting, employing DBSCAN for clustering, and utilizing a specialized Genetic Algorithm for cuboid extraction, this method achieves enhanced stability and robustness. It excels in reconstructing spheres, cylinders, and cuboids from large point sets, with performance metrics and visualizations provided to demonstrate its effectiveness, alongside a discussion on its limitations. For more detailed insights, refer to {% cite friedrich2020hybrid %}.

![Point Cloud Segmentation](\assets\figures\4_point_cloud_segmentation.jpg){:style="display:block; width:80%" .align-center}
