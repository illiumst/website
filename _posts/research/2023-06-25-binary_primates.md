---
layout: single
title:  "Binary Presorting"
categories: research audio deep-learning anomalie-detection 
excerpt: "Improving Primate Sounds Classification"
header:
  teaser: assets/figures/19_binary_primates_teaser.jpg
---

![Multiclass Training Pipeline](\assets\figures\19_binary_primates_pipeline.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

In the field of wildlife observation and conservation, approaches involving machine learning on audio recordings are becoming increasingly popular. Unfortunately, available datasets from this field of research are often not optimal learning material; Samples can be weakly labeled, of different lengths or come with a poor signal-to-noise ratio. In this work, we introduce a generalized approach that first relabels subsegments of MEL spectrogram representations, to achieve higher performances on the actual multi-class classification tasks. For both the binary pre-sorting and the classification, we make use of convolutional neural networks (CNN) and various data-augmentation techniques. We showcase the results of this approach on the challenging ComparE 2021 dataset, with the task of classifying between different primate species sounds, and report significantly higher Accuracy and UAR scores in contrast to comparatively equipped model baselines.
{% cite koelle23primate %}

![Thresholding](\assets\figures\19_binary_primates_thresholding.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

![Thresholding](\assets\figures\19_binary_primates_results.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
