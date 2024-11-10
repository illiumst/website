---
layout: single
title:  "MAS Emergence"
categories: research multi-agent reinforcement-learning safety emergence 
excerpt: "A safety perspective on emergence in multi-agent reinforcement-learning"
header:
  teaser: assets/figures/21_coins_teaser.png
---

![Evaluation Environments](\assets\figures\21_envs.png){:style="display:block; width:40%" .align-right}
Emergent effects can occur in multi-agent systems (MAS), where decision-making is decentralized and based on local information. These effects may range from minor deviations in behavior to catastrophic system failures. To formally define these phenomena, we identify misalignments between the global inherent specification (the true specification) and its local approximation (e.g., the configuration of distinct reward components or observations). Leveraging established safety concepts, we develop a framework for understanding these emergent effects. To demonstrate the resulting implications, we examine two highly configurable gridworld scenarios, where inadequate specifications lead to unintended behavior deviations when derived independently. Acknowledging that a global solution may not always be practical, we propose adjusting the underlying parameterizations to mitigate these issues, thereby improving system alignment and reducing the risk of emergent failures.
{% cite altmann2024emergence %}

![Instances of emergent behavior](\assets\figures\21_coins.png){:style="display:block; width:70%" .align-center}

![Blocking behavior](\assets\figures\21_blocking.png){:style="display:block; width:70%" .align-center}


