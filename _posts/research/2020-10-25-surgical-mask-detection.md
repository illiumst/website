---
layout: single
title: "Surgical-Mask Detection"
categories: research
tags: audio-classification deep-learning data-augmentation computer-vision paralinguistics
excerpt: "CNN mask detection in speech using augmented spectrograms."
header:
  teaser: /assets/figures/7_mask_models.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

This study investigates the efficacy of various **data augmentation techniques** applied directly to **mel-spectrogram representations** of audio data for improving classification performance. The specific task addressed is the detection of surgical mask usage based on human speech signals, a relevant problem in paralinguistics and audio analysis.

We systematically evaluated the impact of data augmentation when training **Convolutional Neural Networks (CNNs)** for this binary classification task. The input to the networks consisted of mel-spectrograms derived from voice samples. The effectiveness of augmentation strategies (such as frequency masking, time masking, or combined approaches like SpecAugment) was assessed across **four different CNN architectures**.

<center>
  <img src="/assets/figures/7_mask_mels.jpg" alt="Examples of mel-spectrograms of speech with and without a surgical mask" style="display:block; width:80%">
  <figcaption>Mel-spectrogram representations of speech signals used as input for CNNs.</figcaption>
</center><br>

The core finding of this research is that applying appropriate data augmentation directly to the spectrogram inputs significantly enhances the performance and generalization capabilities of the CNN models for surgical mask detection. The augmented models demonstrated improved accuracy, robustness, and notably **surpassed many established benchmark results** from the relevant ComParE (Computational Paralinguistics Challenge) tasks. This highlights the importance of data augmentation as a crucial component in building effective deep learning models for audio classification, particularly when dealing with limited or variable datasets. For a detailed description of the methods and results, please refer to {% cite illium2020surgical %}.

<center>
  <img src="/assets/figures/7_mask_models.jpg" alt="Diagrams illustrating the different CNN architectures tested" style="display:block; width:100%">
  <figcaption>Overview of the different Convolutional Neural Network architectures evaluated.</figcaption>
</center>