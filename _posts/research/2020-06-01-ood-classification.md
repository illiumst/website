---
layout: single
title:  "Policy Entropy for OOD Classification"
categories: research 
excerpt: "PEOC for reliably detecting unencountered states in deep RL"
header:
  teaser: assets/figures/6_ood_pipeline.jpg
---

![PEOC Performance](\assets\figures\6_ood_performance.jpg){:style="display:block; width:45%" .align-right}In this work, the development of PEOC, a policy entropy-based classifier for detecting unencountered states in deep reinforcement learning, is proposed. Utilizing the agent's policy entropy as a score, PEOC effectively identifies out-of-distribution scenarios, crucial for ensuring safety in real-world applications. Evaluated against advanced one-class classifiers within procedurally generated environments, PEOC demonstrates competitive performance.
Additionally, a structured benchmarking process for out-of-distribution classification in reinforcement learning is presented, offering a comprehensive approach to evaluating such systems' reliability and effectiveness. {% cite sedlmeier2020policy %}

![PEOC Pipeline](\assets\figures\6_ood_pipeline.jpg){:style="display:block; width:90%" .align-center}
