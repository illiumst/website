---
layout: single
title: "Neural Self-Replication"
categories: research
tags: neural-networks artificial-life complex-systems self-organization
excerpt: "Neural networks replicating weights, inspired by biology and artificial life."
header:
  teaser: /assets/figures/1_self_replication_pca_space.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![alt text](\assets\figures\1_self_replication_robustness.jpg)
{:style="display:block; width:45%" .align-right}

Drawing inspiration from the fundamental process of self-replication in biological systems, this research explores the potential for implementing analogous mechanisms within neural networks. The objective is to develop computational models capable of autonomously reproducing their own structure (specifically, their connection weights), potentially leading to the emergence of complex, adaptive behaviors.

The study investigates various neural network architectures and learning paradigms suitable for achieving self-replication. A key finding highlights the efficacy of leveraging backpropagation-like mechanisms, not for a typical supervised task, but for navigating the weight space in a manner conducive to replication. This approach facilitates the development of non-trivial self-replicating networks.

Furthermore, the research extends this concept by proposing an "artificial chemistry" environment. This framework involves populations of interacting neural networks, where self-replication dynamics can lead to emergent properties and complex ecosystem behaviors. This work offers a novel computational perspective on self-replication, providing tools and insights for exploring artificial life and the principles of self-organization in computational systems. For a detailed discussion, please refer to the publication by {% cite gabor2019self %}.
<div style="clear: both;"></div>

<center>
  <img src="/assets/figures/1_self_replication_pca_space.jpg" alt="PCA visualization showing clusters or trajectories of self-replicating networks in a latent space" style="display:block; width:100%">
  <figcaption>Visualization of self-replicator populations evolving in a PCA-reduced weight space.</figcaption>
</center>