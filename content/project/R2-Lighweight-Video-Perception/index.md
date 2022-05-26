---
title: Flexible Patch Skip for Real-time Visual Perception.
summary: Our research focuses on the software and hardware synergy of on-device learning techniques, covering the scope of model-level neural network design, algorithm-level training optimization and hardware-level arithmetic acceleration.
tags:
- TinyML
date: "2022-04-05"

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

**Illustration:** utilizing the temporal redundancy in video streams to construct efficient on-device video perception systems is a potential approach. We isolate the computation-saving challenge from video perception tasks and offer a task-independent acceleration approach that may be applied across a variety of runtime contexts. By separating acceleration and tasks, we plan to build novel quality-determining criteria for system design and provide an autonomous computation skipping approach to enable different video perception settings. We want to use a learnable gate in each convolution layer to decide which patches may be safely omitted without affecting model accuracy. The gate is optimized by a rigorous self-supervising approach that learns high-level semantics holistically to discern similarity and difference across frames.
Such a small gate architecture is compatible with common edge devices, and it can be used as a plug-and-play module in CNN backbones to provide patch-skippable networks.

