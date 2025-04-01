---
layout: single
title: "ErLoWa Leak Detection"
categories: projects
excerpt: "Deep learning detects acoustic water leaks with SWM."
tags: acoustic anomaly-detection deep-learning real-world-data signal-processing
header:
  teaser: /assets/images/projects/pipe_leak.png # Corrected path
role: Data Scientist, Machine Learning Expert
skills: Acoustic Signal Processing, Deep Learning (CNNs), Anomaly Detection, Real-world Data Handling, Sensor Data Analysis, Industry Collaboration
---

![Leaking pipe icon](/assets/images/projects/pipe_leak.png){: .align-left style="padding:0.1em; width:5em"}
In collaboration with Munich's municipal utility provider, Stadtwerke München (SWM), this project explored the feasibility of using acoustic monitoring for early leak detection in water pipe infrastructure. The primary goal was to develop machine learning models capable of identifying leak-indicating sound patterns within a real-world operational environment.

---

**Project:** ErLoWa (Erkennung von Leckagen in Wasserleitungsnetzen)<br>
**Partner:** [Stadtwerke München (SWM)](https://www.swm.de/)<br>
**Duration:** Late 2018 - Early 2020<br>
**Objective:** To investigate and develop methods for the automated detection and localization of leaks in urban water distribution networks using acoustic sensor data.<br>

---

**Methodology & Activities:**

*   **Data Acquisition:** Sensor networks comprising contact microphones were deployed across sections of Munich's suburban water network to capture continuous acoustic data.
*   **Signal Processing:** Raw audio signals were pre-processed and transformed into mel spectrograms, converting the time-domain audio data into image-like representations suitable for analysis with computer vision techniques.
*   **Model Development:** Various machine learning approaches were evaluated. Deep neural networks, particularly Convolutional Neural Networks (CNNs), were trained on the spectrogram data to classify segments as containing leak sounds or normal background noise.
*   **Analysis & Validation:** The performance of the models was assessed against ground truth data provided by SWM, identifying both the successes and challenges of applying these methods in a complex, noisy, real-world setting.

<center>
    <figure class="half" style="max-width: 70%; text-align:center;">

    <img src="\assets\images\projects\pipe_leak\1fe8265e-ff21-4e9c-8a2a-2ebcaec41728.jpeg"  style="margin-bottom: 0em;">

    <img src="\assets\images\projects\pipe_leak\8d2364f1-1b03-480d-9ed3-09d548f47383.jpeg"  style="margin-bottom: 0em;">

    </figure>
</center><br>

**Key Findings & Outcomes:**

*   The project demonstrated the potential of deep learning models applied to mel spectrograms for identifying relevant acoustic features indicative of water leaks.
*   CNN-based approaches showed advantages over traditional machine learning methods in capturing the complex patterns associated with leak sounds amidst background noise.
*   Significant insights were gained regarding the practical challenges of sensor deployment, data quality variability, and noise interference in real-world utility networks.
*   The research conducted within this project formed the basis for several scientific [publications](/publications) on acoustic anomaly detection. [Paper writeup](/research/acoustic-leak-detection/) for {% cite muller2021acoustic %}

<center>
    <figure class="half" style="max-width: 70%; text-align:center;">

    <img src="\assets\images\projects\pipe_leak\5ea8f0ee-6c61-4835-944c-b77683d397ca.jpeg" style="margin-bottom: 0em;">

    <img src="\assets\images\projects\pipe_leak\cc01cc58-d3f6-4220-b4f4-c7ea26b3a116.jpeg" style="margin-bottom: 0em;">

    </figure>
</center><br>

This applied research project provided valuable experience in handling real-world sensor data, adapting machine learning models for specific industrial challenges, and collaborating effectively with industry partners.

{% include reference.html %}
