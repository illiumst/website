---
layout: single
title:  "Anomalous Image Transfer"
categories: research audio deep-learning anomalie-detection 
excerpt: "Acoustic Anomaly Detection for Machine Sounds based on Image Transfer Learning"
header:
  teaser: assets/figures/9_image_transfer_sound_teaser.jpg
---
![Workflow](\assets\figures\9_image_transfer_sound_workflow.jpg){:style="display:block; width:45%" .align-right}
This paper explores acoustic malfunction detection in industrial machinery using transfer learning, specifically leveraging neural networks pretrained on image classification to extract features. 
These features, when used with anomaly detection models, outperform traditional convolutional autoencoders in noisy conditions across different machine types. The study highlights the superiority of features from ResNet architectures over AlexNet and Squeezenet, with Gaussian Mixture Models and One-Class Support Vector Machines showing the best performance in detecting anomalies.
{% cite muller2020acoustic %}

![Mels](\assets\figures\9_image_transfer_sound_mels.jpg){:style="display:block; width:85%" .align-center}
