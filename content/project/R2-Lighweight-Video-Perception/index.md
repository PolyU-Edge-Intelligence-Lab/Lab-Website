---
title: Task-independent Patch Skip for Real-time Visual Perception.
summary: Our research focuses on the software and hardware synergy of on-device learning techniques, covering the scope of model-level neural network design, algorithm-level training optimization and hardware-level arithmetic acceleration.
tags:
- TinyML
date: "2022-04-17"

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

### Research Opportunity 2: Task-independent Patch Skip for Real-time Visual Perception

**Illustration:** exploiting temporal redundancy in video streams is a promising way to implement efficient on-device video perception systems. We abstract away the computation saving problem from video perception tasks and propose a task-independent acceleration methodology that can generalize to different runtime environments. Following this principle, we intend to develop new quality-determining factors for system design and present an automatic computation skipping method to support diverse video perception settings by decoupling acceleration and tasks. We intend to equip each convolution layer with a learnable gate to selectively determine which patches could be safely skipped without compromising model accuracy. The gate is optimized via a tough self-supervisory procedure and holistically learns high-level semantics to distinguish similarity and difference across frames. The tiny architecture of the gate is compatible with commodity edge devices and can serve as a plug-and-play module in CNN backbones to enable patch-skippable networks. 
