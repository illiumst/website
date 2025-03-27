---
layout: single
title: "Deep Audio Baselines"
categories: research
tags: deep-learning audio-classification paralinguistics speech-analysis
excerpt: "Deep learning audio baseline for Interspeech 2019 ComParE challenge."
header:
  teaser: /assets/figures/3_deep_neural_baselines_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---
![alt text](\assets\figures\3_deep_neural_baselines.jpg)
{:style="display:block; width:30%" .align-right}

This research, presented as part of the Interspeech 2019 Computational Paralinguistics Challenge (ComParE), specifically addresses the Sleepiness Sub-Challenge. We introduced a robust, end-to-end deep learning methodology designed to serve as a strong baseline for audio classification tasks within the paralinguistics domain.

The core innovation lies in utilizing a deep neural network architecture (e.g., CNNs, potentially combined with recurrent layers) that directly processes raw or minimally processed audio data (such as spectrograms). This end-to-end approach bypasses the need for extensive, task-specific manual feature engineering, which is often a complex and time-consuming aspect of traditional audio analysis pipelines.

Our proposed baseline model achieved performance comparable to established state-of-the-art methods on the sleepiness detection task. Furthermore, the architecture was designed with adaptability in mind, demonstrating its potential applicability to a broader range of audio classification challenges beyond sleepiness detection. This work underscores the power of deep learning to automatically extract relevant features from audio signals for complex paralinguistic tasks. For further details, please consult the publication by {% cite elsner2019deep %}.
