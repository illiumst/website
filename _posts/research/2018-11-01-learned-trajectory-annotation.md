---
layout: single
title: "Learned Trajectory Annotation"
categories: research
tags: geoinformatics machine-learning unsupervised-learning human-robot-interaction autoencoder
excerpt: "Unsupervised autoencoder learns spatial context from trajectory data for annotation."
header:
  teaser: /assets/figures/0_trajectory_reconstruction_teaser.png
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

<center>
  <img src="/assets/figures/0_trajectory_isovist.jpg" alt="Visualization of spatial perception field (e.g., isovist) from a point on a trajectory" style="width:48%; display: inline-block; margin: 1%;">
  <img src="/assets/figures/0_trajectory_reconstruction.jpg" alt="Clustered or reconstructed trajectories based on learned spatial representations" style="width:48%; display: inline-block; margin: 1%;">
  <figcaption>Learning spatial context representations (left) enables clustering and annotation of trajectories (right).</figcaption>
</center><br>


This research addresses the challenge of enabling more intuitive human-robot interaction in shared spaces, particularly focusing on grounding verbal communication in spatial understanding. The work introduces a novel unsupervised learning methodology based on neural autoencoders.

The core contribution is a system that learns continuous, low-dimensional representations of spatial context directly from trajectory data, without requiring explicit environmental maps or predefined regions. By processing sequences of spatial perceptions (analogous to visibility fields or isovists) along a path, the autoencoder captures salient environmental features relevant to movement.

These learned latent representations facilitate the effective clustering of trajectories based on shared spatial experiences. The outcome is a set of semantically meaningful encodings and prototypical representations of movement patterns within an environment. This approach lays essential groundwork for developing robotic systems capable of understanding, interpreting, and potentially describing movement through space in human-comprehensible terms, representing a promising direction for future human-robot collaboration. {% cite feld2018trajectory %}

