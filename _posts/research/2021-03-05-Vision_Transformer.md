---
layout: single
title:  "Mel-Vision Transformer"
categories: research audio deep-learning anomalie-detection 
excerpt: "Attention based audio classification on Mel-Spektrograms"
header:
  teaser: assets/figures/12_vision_transformer_teaser.jpg
---

![Leak-Mels](\assets\figures\12_vision_transformer_data.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

We apply the vision transformer, a deep machine learning model build around the attention mechanism, on mel-spectrogram representations of raw audio recordings. When adding mel-based data augmentation techniques and sample-weighting, we achieve comparable performance on both (PRS and CCS challenge) tasks of ComParE21, outperforming most single model baselines. We further introduce overlapping vertical patching and evaluate the influence of parameter configurations.
{% cite illium2021visual %}

![Approach](\assets\figures\12_vision_transformer_models.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
