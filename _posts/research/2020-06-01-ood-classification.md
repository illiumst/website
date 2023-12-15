---
layout: single
title:  "Policy Entropy for OOD Classification"
categories: research 
excerpt: "PEOC for reliably detecting unencountered states in deep RL"
header:
  teaser: assets/figures/6_ood_pipeline.jpg
---

![PEOC Pipeline](\assets\figures\6_ood_pipeline.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

One critical prerequisite for the deployment of reinforcement learning systems in the real world is the ability to reliably detect situations on which the agent was not trained. Such situations could lead to potential safety risks when wrong predictions lead to the execution of harmful actions. In this work, we propose PEOC, a new policy entropy based out-of-distribution classifier that reliably detects unencountered states in deep reinforcement learning. It is based on using the entropy of an agent's policy as the classification score of a one-class classifier. We evaluate our approach using a procedural environment generator. Results show that PEOC is highly competitive against state-of-the-art one-class classification algorithms on the evaluated environments. Furthermore, we present a structured process for benchmarking out-of-distribution classification in reinforcement learning.
{% cite sedlmeier2020peoc %}

![PEOC Performance](\assets\figures\6_ood_performance.jpg){:style="display:block; margin-left:auto; margin-right:auto"}


