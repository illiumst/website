---
layout: single
title: "Soccer Team Vectors"
categories: research
tags: machine-learning representation-learning sports-analytics similarity-search
excerpt: "STEVE learns soccer team embeddings from match data for analysis."
header:
  teaser: /assets/figures/2_steve_algo.jpg
scholar_link: "https://scholar.google.de/citations?user=NODAd94AAAAJ&hl=en"
---
This research introduces **STEVE (Soccer Team Vectors)**, a novel methodology for learning meaningful, real-valued vector representations (embeddings) for professional soccer teams. The primary goal is to capture intrinsic team characteristics and relationships within a continuous vector space, such that teams with similar playing styles, strengths, or performance levels are positioned closely together.

Leveraging widely available public data from soccer matches (e.g., results, possibly performance statistics), STEVE employs machine learning techniques to generate these low-dimensional team vectors.

The utility of these learned representations is demonstrated through several downstream applications:

![alt text](\assets\figures\2_steve_algo.jpg){:style="display:block; width:60%" .align-right}

*   **Team Market Value Estimation:** The vectors serve as effective features for predicting team market values, outperforming baseline models.
*   **Similarity Search:** The vector space allows for efficient identification of teams similar to a given query team based on proximity.
*   **Team Ranking:** The embeddings provide a basis for generating data-driven team rankings.

Across these application domains, STEVE demonstrated superior performance compared to competing approaches evaluated in the study. This work provides a valuable tool for quantitative analysis in sports analytics, enabling various machine learning tasks related to team comparison and prediction. For a comprehensive description of the methodology and results, please refer to the publication by {% cite muller2020soccer %}.