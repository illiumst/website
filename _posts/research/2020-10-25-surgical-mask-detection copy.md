---
layout: single
title:  "Surgical Mask Detection"
categories: research audio deep-learning
excerpt: "Convolutional Neural Networks and Data Augmentations on Spectrograms"
header:
  teaser: assets/figures/7_mask_models.jpg
---

![PEOC Pipeline](\assets\figures\7_mask_mels.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

In many fields of research, labeled data-sets are hard to acquire. This is where data augmentation promises to overcome the lack of training data in the context of neural network engineering and classification tasks. The idea here is to reduce model over-fitting to the feature distribution of a small under-descriptive training data-set. We try to evaluate such data augmentation techniques to gather insights in the performance boost they provide for several convolutional neural networks on mel-spectrogram representations of audio data. We show the impact of data augmentation on the binary classification task of surgical mask detection in samples of human voice. Also we consider four varying architectures to account for augmentation robustness. Results show that most of the baselines given by ComParE are outperformed
{% cite illium2020surgical %}

![Models](\assets\figures\7_mask_models.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
