---
layout: single
title:  "Binary Presorting"
categories: research audio deep-learning anomalie-detection 
excerpt: "Improving primate sounds classification by sublabeling"
header:
  teaser: assets/figures/19_binary_primates_teaser.jpg
---

![Multiclass Training Pipeline](\assets\figures\19_binary_primates_pipeline.jpg){:style="display:block; width:40%" .align-right}
This study advances machine learning applications in wildlife observation by introducing a sophisticated approach to audio classification. By meticulously relabeling subsegments of MEL spectrograms, it significantly refines the process of multi-class classification, crucial for identifying various primate species from audio recordings. Employing convolutional neural networks alongside innovative data augmentation techniques, the methodology showcases remarkable enhancements in classification performance. When applied to the demanding ComparE 2021 dataset, this approach not only achieved substantially higher accuracy and UAR scores over existing baselines but also marked a significant stride in the field of bioacoustics research, demonstrating the potential of machine learning to overcome challenges presented by datasets with weak labeling, varying lengths, and poor signal-to-noise ratios.
{% cite koelle23primate %}

![Thresholding](\assets\figures\19_binary_primates_thresholding.jpg){:style="display:block; width:70%" .align-center}

![Thresholding](\assets\figures\19_binary_primates_results.jpg){:style="display:block; width:70%" .align-center}
