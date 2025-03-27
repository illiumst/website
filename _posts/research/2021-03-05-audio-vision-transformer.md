---
layout: single
title: "Audio Vision Transformer"
categories: research
tags: deep-learning audio-classification computer-vision attention-mechanisms transformers
excerpt: "Vision Transformer on spectrograms for audio classification, with data augmentation."
header:
  teaser: /assets/figures/12_vision_transformer_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

This research explores the application of the **Vision Transformer (ViT)** architecture, originally designed for image processing, to the domain of audio classification by operating on **mel-spectrogram representations**. The ViT's attention mechanisms offer a potentially powerful alternative to convolutional approaches for capturing relevant patterns in spectrogram data.

<center>
  <img src="/assets/figures/12_vision_transformer_models.jpg" alt="Diagram illustrating the Vision Transformer architecture adapted for mel-spectrogram input" style="display:block; width:80%">
  <figcaption>Adapting the Vision Transformer architecture for processing mel-spectrograms.</figcaption>
</center><br>


Key aspects of the methodology include:

*   **ViT Adaptation:** Applying the ViT model directly to mel-spectrograms treated as images.
*   **Data Augmentation:** Employing **mel-based data augmentation** techniques (e.g., SpecAugment variants) to improve model robustness and generalization.
*   **Sample Weighting:** Utilizing sample weighting strategies to address potential class imbalances or focus on specific aspects of the dataset.
*   **Patching Strategy:** Introducing and evaluating an **overlapping vertical patching** method, potentially better suited for capturing temporal structures in spectrograms compared to standard non-overlapping patches.

The effectiveness of this "Mel-Vision Transformer" approach was demonstrated within the context of the **ComParE 2021 (Computational Paralinguistics Challenge)**. The proposed model achieved notable performance, **surpassing many established single-model baseline results** on the challenge tasks.

Furthermore, the study includes an analysis of different parameter configurations and architectural choices, providing insights into optimizing ViT models for audio processing tasks. This work showcases the adaptability and potential of transformer architectures, particularly ViT, for effectively tackling audio classification challenges. {% cite illium2021visual %}