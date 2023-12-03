---
layout: single
title:  "Primate Vocalization Classification"
categories: research audio deep-learning anomalie-detection 
excerpt: "A Deep and Recurrent Architecture"
header:
  teaser: assets/figures/11_recurrent_primate_workflow.jpg
---

![Leak-Mels](\assets\figures\11_recurrent_primate_workflow.jpg){:style="display:block; margin-left:auto; margin-right:auto"}

Wildlife monitoring is an essential part of most conservation efforts where one of the many building blocks is acoustic monitoring. Acoustic monitoring has the advantage of being noninvasive and applicable in areas of high vegetation. In this work, we present a deep and recurrent architecture for the classification of primate vocalizations that is based upon well proven modules such as bidirectional Long Short-Term Memory neural networks, pooling, normalized softmax and focal loss. Additionally, we apply Bayesian optimization to obtain a suitable set of hyperparameters. We test our approach on a recently published dataset of primate vocalizations that were recorded in an African wildlife sanctuary.
{% cite muller2021deep %}

![Approach](\assets\figures\11_recurrent_primate_results.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
