---
layout: single
title: "Sound Anomaly Transfer"
categories: research
tags: anomaly-detection audio-classification deep-learning transfer-learning feature-extraction computer-vision
excerpt: "Image nets detect acoustic anomalies in machinery via spectrograms."
header:
  teaser: /assets/figures/9_image_transfer_sound_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Workflow diagram showing mel-spectrogram input, feature extraction via image network, and anomaly detection model](\assets\figures\9_image_transfer_sound_workflow.jpg)
{:style="display:block; width:45%" .align-right}


This study investigates an effective approach for **acoustic anomaly detection** in industrial machinery, focusing on identifying malfunctions through sound analysis. The core methodology leverages **transfer learning** by repurposing deep neural networks originally trained for large-scale **image classification** (e.g., on ImageNet) as powerful feature extractors for audio data represented as **mel-spectrograms**.

The process involves:
1.  Converting audio signals from machinery into mel-spectrogram images.
2.  Feeding these spectrograms into various pretrained image classification networks (specifically comparing **ResNet architectures** against **AlexNet** and **SqueezeNet**) to extract deep feature representations.
3.  Training standard anomaly detection models – particularly **Gaussian Mixture Models (GMMs)** and **One-Class Support Vector Machines (OC-SVMs)** – on the features extracted from normal operation sounds.
4.  Classifying new sounds as anomalous if their extracted features deviate significantly from the learned normality model.

Key findings from the experiments, conducted across different machine types and noise conditions, include:

*   The proposed transfer learning approach significantly **outperforms baseline methods like traditional convolutional autoencoders**, especially in the presence of background noise.
*   Features extracted using **ResNet architectures consistently yielded superior anomaly detection performance** compared to those from AlexNet and SqueezeNet.
*   **GMMs and OC-SVMs proved highly effective** as anomaly detection classifiers when applied to these transferred features.

<div style="clear: both;"></div>

<center>
  <img src="/assets/figures/9_image_transfer_sound_mels.jpg" alt="Examples of mel-spectrograms from normal and anomalous machine sounds" style="display:block; width:85%">
  <figcaption>Mel-spectrogram examples of normal vs. anomalous machine sounds.</figcaption>
</center>


This work demonstrates the surprising effectiveness of transferring knowledge from the visual domain to the acoustic domain for anomaly detection, offering a robust and readily implementable method for monitoring industrial equipment. {% cite muller2020acoustic %}