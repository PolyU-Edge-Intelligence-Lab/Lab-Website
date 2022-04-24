---
title: Adaptive Quantization-aware Training and Model Compression.
summary: Our research focuses on the software and hardware synergy of on-device learning techniques, covering the scope of model-level neural network design, algorithm-level training optimization and hardware-level arithmetic acceleration.
tags:
- TinyML
date: "2022-04-18"

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

### Research Opportunity 1: Adaptive Quantization-aware Training and Model Compression

**Illustration:** On-device learning is an emerging technique to pave the last mile of enabling edge intelligence, which eliminates the limitations of conventional in-cloud computing where dozens of computational capacities and memories are needed. A high- performance on-device learning system requires breaking the constraints of limited resources and alleviating computational overhead. Our preliminary work shows that employing the 8-bit fixed-point (INT8) quantization in both forward and back- ward passes over a deep model is a promising way to enable tiny on-device learning in practice. The key to an efficient quantization-aware training (QAT) method is to exploit the hardware- level enabled acceleration while preserving the training quality in each layer. However, off-the-shelf quantization methods cannot handle the on-device learning paradigm of fixed-point processing. To overcome these challenges, we propose to design an adaptive QAT algorithm, which jointly optimizes the computation of forward and backward passes. Besides, we need to build efficient network components to automatically counteract the quantization error of tensor arithmetic. We intend to implement our methods in Octo, a lightweight cross-platform system for tiny on-device learning, and keep improving its performance to support more realistic applications.
