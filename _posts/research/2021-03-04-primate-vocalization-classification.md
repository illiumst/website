---
layout: single
title: "Primate Vocalization Classification"
categories: research
tags: deep-learning audio-classification bioacoustics conservation-technology recurrent-neural-networks
excerpt: "Deep BiLSTM classifies primate vocalizations for acoustic wildlife monitoring."
header:
  teaser: /assets/figures/11_recurrent_primate_workflow.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Workflow diagram showing audio input, feature extraction, BiLSTM processing, and classification output](\assets\figures\11_recurrent_primate_workflow.jpg)
{:style="display:block; width:40%" .align-right}

Acoustic monitoring offers a powerful, non-invasive tool for wildlife conservation, enabling the study and tracking of animal populations through their vocalizations. This research focuses on improving the automated classification of **primate vocalizations**, a challenging task due to call variability and environmental noise.

We propose a novel **deep, recurrent neural network architecture** specifically designed for this purpose. The core of the model utilizes **bidirectional Long Short-Term Memory (BiLSTM) networks**, which are adept at capturing temporal dependencies within the audio signals (represented, for example, as spectrograms or MFCCs).

To further enhance classification performance, particularly in potentially imbalanced datasets common in bioacoustics, the architecture incorporates advanced techniques:
*   **Normalized Softmax:** Improves calibration and potentially robustness.
*   **Focal Loss:** Addresses class imbalance by focusing training on hard-to-classify examples.

Hyperparameter tuning, a critical step for optimizing deep learning models, was systematically performed using **Bayesian optimization**.

<center>
  <img src="/assets/figures/11_recurrent_primate_results.jpg" alt="Graph or table showing classification accuracy or confusion matrix for primate calls" style="display:block; width:90%">
  <figcaption>Performance results demonstrating classification accuracy.</figcaption>
</center><br>

The model's effectiveness was evaluated on a challenging real-world dataset comprising diverse primate calls recorded at an **African wildlife sanctuary**. The results demonstrate the capability of the proposed deep recurrent architecture for accurate primate vocalization classification, underscoring the potential of advanced deep learning techniques combined with automated acoustic monitoring for practical wildlife conservation efforts. {% cite muller2021deep %}