---
layout: single
title: "Aquarium MARL Environment"
categories: research
tags: multi-agent-reinforcement-learning MARL simulation emergence complex-systems
excerpt: "Aquarium: Open-source MARL environment for predator-prey studies."
header:
  teaser: /assets/figures/20_aquarium.png
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

![Diagram illustrating the multi-agent reinforcement learning cycle within the Aquarium environment](\assets\figures\20_aquarium.png){:style="display:block; width:40%" .align-right}

The study of complex interactions using Multi-Agent Reinforcement Learning (MARL), particularly **predator-prey dynamics**, often requires specialized simulation environments. To streamline research and avoid redundant development efforts, we introduce **Aquarium**: a versatile, open-source MARL environment specifically designed for investigating predator-prey scenarios and related **emergent behaviors**.

Key Features of Aquarium:

*   **Framework Integration:** Built upon and seamlessly integrates with the popular **PettingZoo API**, allowing researchers to readily apply existing MARL algorithm implementations (e.g., from Stable-Baselines3, RLlib).
*   **Physics-Based Movement:** Simulates agent movement on a two-dimensional, continuous plane with edge-wrapping boundaries, incorporating basic physics for more realistic interactions.
*   **High Customizability:** Offers extensive configuration options for:
    *   **Agent-Environment Interactions:** Observation spaces, action spaces, and reward functions can be tailored to specific research questions.
    *   **Environmental Parameters:** Key dynamics like agent speeds, prey reproduction rates, predator starvation mechanisms, sensor ranges, and more are fully adjustable.
*   **Visualization & Recording:** Includes a resource-efficient visualizer and supports video recording of simulation runs, facilitating qualitative analysis and understanding of agent behaviors.

<div style="display: flex; align-items: center; justify-content: center;">
  <center>
    <img src="/assets/figures/20_observation_vector.png" alt="Diagram detailing the construction of the observation vector for an agent" style="display:inline-table; width:85%">
    <figcaption>Construction details of the agent observation vector.</figcaption>
  </center>
  <center>
    <img src="/assets/figures/20_capture_statistics.png" alt="Graphs showing average captures or rewards per prey agent under different training regimes" style="display:inline-table; width:100%">
    <figcaption>Performance metrics (e.g., average captures/rewards) comparing training strategies.</figcaption>
  </center>
</div>

To demonstrate its capabilities, we conducted preliminary studies using **Proximal Policy Optimization (PPO)** to train multiple prey agents learning to evade a predator within Aquarium. Consistent with findings in existing MARL literature, our results showed that training agents with **individual policies led to suboptimal performance**, whereas utilizing **parameter sharing** among prey agents significantly improved coordination, sample efficiency, and overall evasion success. {% cite kolle2024aquarium %}
