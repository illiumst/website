---
layout: single
title: "Tasked Self-Replication"
categories: research
tags: artificial-life complex-systems neural-networks self-organization multi-task-learning
excerpt: "Self-replicating networks perform tasks, exploring stabilization in artificial chemistry."
header:
  teaser: /assets/figures/13_sr_teaser.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

Building upon the concept of self-replicating neural networks, this research explores the integration of **auxiliary functional goals** alongside the primary objective of self-replication. The aim is to create networks that can not only reproduce their own weights but also perform useful computations or interact meaningfully with an environment simultaneously.

<center>
  <img src="/assets/figures/13_sr_analysis.jpg" alt="Analysis graphs or visualizations related to dual-task self-replicating networks" style="display:block; width:80%">
  <figcaption>Analysis of networks balancing self-replication and auxiliary tasks.</figcaption>
</center><br>

The study introduces a methodology for **dual-task training**, utilizing distinct input/output vectors to manage both the replication process and the execution of a secondary task. A key finding is that the presence of an auxiliary task does not necessarily hinder self-replication; instead, it can sometimes **complement and even stabilize** the replication dynamics.

Further investigations were conducted within the framework of an **"artificial chemistry" environment**, where populations of these dual-task networks interact:

*   The impact of varying **action parameters** (related to the secondary task) on the collective learning or emergent behavior of the network population was examined.
*   A concept of a specially designed **"guiding particle"** network was introduced. This network influences its peers, demonstrating a mechanism for potentially steering the population's evolution towards desired goal-oriented behaviors.

This work provides insights into how functional complexity can be integrated with self-replication in computational systems, offering potential pathways for developing more sophisticated artificial life models and exploring guided evolution within network populations. {% cite gabor2021goals %}