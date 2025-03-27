---
layout: single
title: "Acoustic Leak Detection"
categories: research
tags: anomaly-detection audio-processing deep-learning signal-processing real-world-application
excerpt: "Anomaly detection models for acoustic leak detection in water networks."
header:
  teaser: /assets/figures/10_water_networks_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Diagram illustrating the anomaly detection approach for leak detection](\assets\figures\10_water_networks_approach.jpg)
{:style="display:block; width:40%" .align-right}

Detecting leaks in vast municipal water distribution networks is critical for resource conservation and infrastructure maintenance. This study introduces and evaluates an **anomaly detection approach for acoustic leak identification**, specifically designed with **energy efficiency** and **ease of deployment** as key considerations.

The methodology leverages acoustic recordings captured by microphones deployed directly on a section of a real-world **municipal water network**. Instead of requiring continuous monitoring, the proposed system mimics human inspection routines by performing **intermittent checks**, significantly reducing power consumption and data load.

Various **anomaly detection models**, ranging from traditional "shallow" methods (e.g., GMMs, OC-SVMs) to more complex **deep learning architectures** (e.g., autoencoders, potentially CNNs on spectrograms), were trained using data representing normal network operation. These models were then evaluated on their ability to distinguish anomalous sounds indicative of leaks.

Key findings include:
*   Detecting leaks occurring acoustically **nearby** the sensor proved relatively straightforward for most evaluated models.
*   **Neural network-based methods demonstrated superior performance** in identifying leaks originating **further away** from the sensor, showcasing their ability to capture more subtle acoustic signatures amidst background noise.

<center>
  <img src="/assets/figures/10_water_networks_mel.jpg" alt="Mel-spectrogram examples showing acoustic signatures of normal operation versus leak sounds" style="display:block; width:90%">
  <figcaption>Mel-spectrogram visualizations comparing normal sounds and leak-related acoustic patterns.</figcaption>
</center><br>

This research validates the feasibility of using anomaly detection for practical, energy-efficient acoustic leak monitoring in water networks, highlighting the advantages of deep learning techniques for detecting more challenging, distant leaks. {% cite muller2021acoustic %}
