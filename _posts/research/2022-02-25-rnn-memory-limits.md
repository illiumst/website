---
layout: single
title: "RNN Memory Limits"
categories: research
tags: deep-learning recurrent-neural-networks sequence-modeling theoretical-ml
excerpt: "Investigated memory limits of RNNs in recalling uncorrelated sequences."
header:
  teaser: /assets/figures/22_rnn_limits.png
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---

Recurrent Neural Networks (RNNs), including variants like Long Short-Term Memory (LSTM) and Gated Recurrent Units (GRU), are designed with the intent to capture temporal dependencies within sequential data. Their internal mechanisms allow information from previous time steps to influence current processing.

This research investigates the fundamental memory capacity of these architectures under challenging conditions: specifically, when processing sequences where data points are generated independently, possessing **no inherent temporal correlation**. In such scenarios, any recall of past inputs relies solely on the network's ability to explicitly memorize information through standard backpropagation training, rather than leveraging statistical patterns in the sequence.

Our empirical analysis demonstrates that while RNNs *can* learn to recall a limited number of past inputs even from uncorrelated sequences, this capability is significantly constrained:

*   **Limited Recall Range:** The effective range over which vanilla RNNs, LSTMs, and GRUs can reliably reproduce past inputs from uncorrelated data is substantially shorter than the recall range achievable when even minimal temporal correlations are present.
*   **Architectural Influence:** This limitation is influenced by both the specific RNN architecture (vanilla, LSTM, GRU) and the network size (number of hidden units).
*   **Practical Bound:** The findings suggest a practical upper bound on the temporal memory achievable through standard training in these scenarios, which appears well below theoretical information storage limits.

<center>
  <img src="/assets/figures/22_rnn_limits.png" alt="Clearly visible memory horizon, established by emperical analysis of an atomic experriment." style="display:block; width:100%">
  <figcaption>RNN Memory Horizon.</figcaption>
</center><br>

These results highlight an inherent constraint in the capacity of standard RNN architectures to identify and utilize long-range dependencies when processing sequences lacking temporal structure, providing insights into their limitations in specific types of sequence modeling tasks. {% cite illium2022empirical %}
