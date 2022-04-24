---
title: Progressive Network Sparsification and Latent Feature Compression for Scalable Collaborative Learning.
summary: Our research focuses on the software and hardware synergy of on-device learning techniques, covering the scope of model-level neural network design, algorithm-level training optimization and hardware-level arithmetic acceleration.
tags:
- TinyML
date: "2022-04-15"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: A Unified TinyML System for Multi-modal Edge Intelligence and Real-time Visual Perception
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""
---

### Research Opportunity 4: Progressive Network Sparsification and Latent Feature Compression for Scalable Collaborative Learning

**Illustration:** In the edge intelligence environment, new data is continuously generated on user devices that cannot be aggregated at once due to privacy and energy concerns. These issues require us to develop new insights into traffic saving to build a communication-efficient collaborative learning paradigm. Unlike previous methods aiming at improving bandwidth utilization or using an unstructured pixel-wise compression, we jointly capture the channel and spatial-level feature redundancy, and conduct a hierarchical compression in these two levels to achieve a much higher traffic reduction ratio. Specifically, we need to design a more efficient feature compression method to leverage the pixel similarity, and reorganize the features into groups based on channel significance to prune the network. Meanwhile, we intend to calibrate the gradients of compressed features with a comprehensive theoretical analysis of the convergence rate. Such a co-design can provide a significant traffic reduction over existing methods while not sacrificing much model accuracy, achieving good training flexibility and communicational efficiency. We believe this work can contribute to the further development of edge intelligence applications.