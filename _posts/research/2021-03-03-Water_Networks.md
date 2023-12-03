---
layout: single
title:  "Acoustic Leak Detection"
categories: research audio deep-learning anomalie-detection 
excerpt: "Anomalie based Leak Detection in Water Networks"
header:
  teaser: assets/figures/10_water_networks_teaser.jpg
---

![Leak-Mels](\assets\figures\10_water_networks_mel.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

In industrial applications, the early detection of malfunctioning factory machinery is crucial. In this paper, we consider acoustic malfunction detection via transfer learning. Contrary to the majority of current approaches which are based on deep autoencoders, we propose to extract features using neural networks that were pretrained on the task of image classification. We then use these features to train a variety of anomaly detection models and show that this improves results compared to convolutional autoencoders in recordings of four different factory machines in noisy environments. Moreover, we find that features extracted from ResNet based networks yield better results than those from AlexNet and Squeezenet. In our setting, Gaussian Mixture Models and One-Class Support Vector Machines achieve the best anomaly detection performance.
{% cite muller2021acoustic %}

![Approach](\assets\figures\10_water_networks_approach.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
