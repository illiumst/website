---
layout: single
title: "Anomalous Sound Features"
categories: research
tags: anomaly-detection audio-classification deep-learning transfer-learning feature-extraction
excerpt: "Pretrained networks extract features for anomalous industrial sound detection."
header:
  teaser: /assets/figures/8_anomalous_sound_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Diagram showing features extracted by different pretrained networks visualized in a latent space](\assets\figures\8_anomalous_sound_features.jpg)
{:style="display:block; width:40%" .align-right}

Detecting anomalous sounds, particularly in industrial settings, is crucial for predictive maintenance and safety. This often involves unsupervised or semi-supervised approaches where models learn a representation of 'normal' sounds. This research explores the effectiveness of leveraging **transfer learning** for this task by using **pretrained deep neural networks** as fixed feature extractors.

The core methodology involves:
1.  Taking pretrained networks trained on large datasets from various domains.
2.  Using these networks to extract high-level, potentially semantically rich feature vectors from audio signals (specifically, industrial machine noises relevant to challenges like DCASE - Detection and Classification of Acoustic Scenes and Events).
3.  Modeling the distribution of features extracted from 'normal' sounds using a **Gaussian Mixture Model (GMM)**.
4.  Identifying anomalous sounds as those whose extracted features have low likelihood under the learned normality model.

A key aspect of this study was comparing feature extractors pretrained on distinctly different domains:
*   **Images** (e.g., models trained on ImageNet)
*   **Environmental Sounds** (e.g., models trained on AudioSet or ESC-50)
*   **Music** (e.g., models trained on music tagging datasets)

These were evaluated alongside a baseline autoencoder trained directly on the target machine sound data.

Surprisingly, the results indicated that features derived from networks pretrained on **music data** often yielded the best performance in detecting anomalous industrial sounds, frequently surpassing features from environmental sound models and the autoencoder baseline. This counter-intuitive finding suggests that direct domain similarity between the pretraining dataset and the target application data is not necessarily the primary factor determining the utility of transferred features for anomaly detection. {% cite muller2020analysis %}
