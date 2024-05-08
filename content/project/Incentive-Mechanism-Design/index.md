---
title: Lack of participants- Incentive Mechanism Design for Federated Learning
summary: A few of works have designed incentive mechanisms for FL, but these mechanisms only consider myopia optimization on resource consumption, which results in the lack of learning algorithm performance guarantee and long-term sustainability. We propose Chiron, an incentive-driven long-term mechanism for edge learning based on hierarchical deep reinforcement learning. 

tags:
- Federated Learning
date: "2022-03-15"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
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

## Introduction

The main objective of incentive is to motive data owners to participate in FL. A few of works have designed incentive mechanisms for FL, but these mechanisms only consider myopia optimization on resource consumption, which results in the lack of learning algorithm performance guarantee and long-term sustainability. We propose Chiron, an incentive-driven long-term mechanism for edge learning based on hierarchical deep reinforcement learning. First, our optimization goal combines learning-algorithms metric (i.e., model accuracy) with system metric (i.e., learning time, and resource consumption), which can improve edge learning quality under a fixed training budget. Second, we present a two-layer H-DRL design with exterior and inner agents to achieve both long-term and short-term optimization for edge learning, respectively.

<!-- {{< figure src="incentive-2.png" caption="Our work: Hierarchical Reinforcement Learning for Incentive mechanism in Federated Learning [6]." >}} -->

##### Reference:

[6]. Incentive-Driven Long-term Optimization for Edge Learning by Hierarchical Reinforcement Mechanism. *ICDCS*, <u>CCF-B</u>