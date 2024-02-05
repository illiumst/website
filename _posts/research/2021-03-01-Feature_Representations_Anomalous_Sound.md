---
layout: single
title:  "Anomalous Sound Detection"
categories: research audio deep-learning anomalie-detection
excerpt: "Analysis of Feature Representations for Anomalous Sound Detection"
header:
  teaser: assets/figures/8_anomalous_sound_teaser.jpg
---

![Pipeline](\assets\figures\8_anomalous_sound_features.jpg){:style="display:block; width:40%" .align-right}
This study explores the use of pretrained neural networks as feature extractors for detecting anomalous sounds, utilizing these networks to derive semantically rich features for a Gaussian Mixture Model that estimates normality. It examines extractors trained on diverse data domains—images, environmental sounds, and music—applied to industrial noises from machinery. Surprisingly, features based on music data often surpass others, including an autoencoder baseline, suggesting that domain similarity between extractor training and application might not always correlate with performance improvement.
{% cite muller2020analysis %}
