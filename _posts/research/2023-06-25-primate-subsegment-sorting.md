---
layout: single
title: "Primate Subsegment Sorting"
categories: research
tags: bioacoustics audio-classification deep-learning data-labeling signal-processing
excerpt: "Binary subsegment presorting improves noisy primate sound classification."
header:
  teaser: /assets/figures/19_binary_primates_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Diagram illustrating the multi-class training pipeline incorporating subsegment relabeling](\assets\figures\19_binary_primates_pipeline.jpg)
{:style="display:block; width:40%" .align-right}

Automated acoustic classification plays a vital role in wildlife monitoring and bioacoustics research. This study introduces a sophisticated pre-processing and training strategy to significantly enhance the accuracy of multi-class audio classification, specifically targeting the identification of different primate species from field recordings.

A key challenge in bioacoustics is dealing with datasets containing weak labels (where calls of interest occupy only a portion of a labeled segment), varying segment lengths, and poor signal-to-noise ratios (SNR). Our approach addresses this by:

1.  **Subsegment Analysis:** Processing audio recordings represented as **MEL spectrograms**.
2.  **Refined Labeling:** Meticulously **relabeling subsegments** within the spectrograms. This "binary presorting" step effectively identifies and isolates the actual vocalizations of interest within longer, weakly labeled recordings.
3.  **CNN Training:** Training **Convolutional Neural Networks (CNNs)** on these refined, higher-quality subsegment inputs.
4.  **Data Augmentation:** Employing innovative **data augmentation techniques** suitable for spectrogram data to further improve model robustness.

<center>
  <img src="/assets/figures/19_binary_primates_thresholding.jpg" alt="Visualization related to the thresholding or selection process for subsegment labeling" style="display:block; width:70%">
  <figcaption>Thresholding or selection criteria for subsegment refinement.</figcaption>
</center><br>

The effectiveness of this methodology was evaluated on the challenging **ComParE 2021 Primate dataset**. The results demonstrate remarkable improvements in classification performance, achieving substantially higher accuracy and Unweighted Average Recall (UAR) scores compared to existing baseline methods.

<center>
  <img src="/assets/figures/19_binary_primates_results.jpg" alt="Graphs or tables showing improved classification results (accuracy, UAR) compared to baselines" style="display:block; width:70%">
  <figcaption>Comparative performance results on the ComParE 2021 dataset.</figcaption>
</center><br>

This work represents a significant advancement in handling difficult, real-world bioacoustic data, showcasing how careful data refinement prior to deep learning model training can dramatically enhance classification outcomes. {% cite koelle23primate %}
