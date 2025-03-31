---
layout: single
title: "Autoencoder Trajectory Compression"
categories: research deep-learning recurrent-neural-networks trajectory-analysis data-compression geoinformatics
excerpt: "Introduced an LSTM autoencoder approach for GPS trajectory compression, demonstrating superior reconstruction accuracy compared to Douglas-Peucker based on Fréchet distance and DTW."
header:
  teaser: /assets/figures/23_trajectory_model.png
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

The proliferation of location-aware mobile devices generates vast amounts of GPS trajectory data, necessitating efficient storage solutions. While various compression techniques aim to reduce data volume, preserving essential spatio-temporal information remains crucial.

<center>
  <img src="/assets/figures/23_trajectory_model.png" alt="Schematic diagram of the LSTM autoencoder model architecture used for trajectory compression" style="display:block; width:60%">
  <figcaption>Schematic of the LSTM Decoder Architecture.</figcaption>
</center>
<br>

This paper introduces a novel approach for **compressing and reconstructing GPS trajectories** using a **Long Short-Term Memory (LSTM) autoencoder**. The autoencoder learns a compressed latent representation of the trajectory sequence, which can then be decoded to reconstruct the original path.

![Graphs showing mean distance errors (e.g., Fréchet, DTW) for different compression ratios on the T-Drive dataset](\assets\figures\23_trajectory_scores.png){:style="display:block; width:50%" .align-right}

Our method was evaluated on two distinct datasets: one from a gaming context and another real-world dataset (T-Drive). We assessed performance across a range of compression ratios and trajectory lengths, comparing it against the widely used traditional **Douglas-Peucker algorithm**.

**Key findings:**

*   The LSTM autoencoder approach significantly **outperforms Douglas-Peucker** in terms of reconstruction accuracy, as measured by both **discrete Fréchet distance** and **Dynamic Time Warping (DTW)**.
*   Unlike point-reduction techniques like Douglas-Peucker, our method performs a **lossy reconstruction at every point** along the trajectory. This offers potential advantages in maintaining temporal resolution and providing greater flexibility for downstream analysis.

Experimental results demonstrate the effectiveness and potential benefits of using deep learning, specifically LSTM autoencoders, for GPS trajectory compression, offering improved accuracy over conventional geometric algorithms. {% cite kolle2023compression %}

