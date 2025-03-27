---
layout: single
title: "PEOC OOD Detection"
categories: research
tags: deep-reinforcement-learning out-of-distribution-detection ai-safety anomaly-detection
excerpt: "PEOC uses policy entropy for OOD detection in deep RL."
header:
  teaser: /assets/figures/6_ood_pipeline.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Graph comparing PEOC performance against other OOD detection methods](\assets\figures\6_ood_performance.jpg)
{:style="display:block; width:45%" .align-right}

Ensuring the safety and reliability of deep reinforcement learning (RL) agents deployed in real-world environments necessitates the ability to detect when the agent encounters states significantly different from those seen during training (i.e., out-of-distribution or OOD states). This research introduces **PEOC (Policy Entropy-based OOD Classifier)**, a novel and computationally efficient method designed for this purpose.

The core idea behind PEOC is to leverage the entropy of the agent's learned policy as an intrinsic indicator of state familiarity. High policy entropy often correlates with uncertainty, suggesting the agent is in a less familiar or potentially OOD state. PEOC utilizes this readily available metric as a scoring function to distinguish between in-distribution and out-of-distribution inputs.

PEOC's effectiveness was rigorously evaluated within procedurally generated environments, which allow for controlled introduction of novel states. Its performance was benchmarked against several state-of-the-art one-class classification methods adapted for the RL context. The results demonstrate that PEOC achieves competitive performance in identifying OOD states while being simple to implement and integrate into existing deep RL frameworks.

Furthermore, this work contributes a structured benchmarking process specifically designed for evaluating OOD classification methods within the context of reinforcement learning, providing a valuable framework for assessing the reliability of such safety-critical components. For a detailed methodology and evaluation, please refer to the publication by {% cite sedlmeier2020policy %}.


<div style="clear: both;"></div>

<figure style="display:block; width:90%; margin: 1em auto; text-align: center;">
  <img src="/assets/figures/6_ood_pipeline.jpg" alt="Diagram showing the PEOC pipeline integrated with a deep RL agent" style="display:block; width:90%">
  <figcaption>Conceptual pipeline of the PEOC method for OOD detection in deep RL.</figcaption>
</figure>