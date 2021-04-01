---
title: Federated Learning in Resourced Constrained Mobile Edge Network
summary: Federated learning (FL) has been proposed as a promising solution for future AI applications with strong privacy protection. It enables distributed computing nodes to collaboratively train models without exposing their own data.
tags:
- Federated Learning
date: "2016-01-01"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Federated Learning Process
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

Federated learning (FL) has been proposed as a promising solution for future AI applications with strong privacy protection. It enables distributed computing nodes to collaboratively train models without exposing their own data. In this research topic, we focus on overcoming the heterogeneity challenge (e.g., data heterogeneity, model heterogeneity) in FL.

{{< figure src="picture1.svg" caption="Collaborative Learning" >}}

Efficient Federated Learning on Heterogeneous Data: from the perspective of distribution characteristics of training data, FL can be categorized into two types, i.e., horizontal federated learning (HFL) and vertical federated learning (VFL). In HFL, we aim to propose efficient and robust learning scheme in resource-constrained computing environment by training a reinforcement learning model to adaptively tune the systematical parameters (e.g., the batch size in each client). Moreover, we explore the unbalanced features in VFL, the fundamental theories and algorithms are proposed to improve the learning efficiency and accuracy.

{{< figure src="picture2.svg" caption="Knowledge Distillation" >}}

The Optimization of Federated Learning with Heterogenous Models: in this topic, we make effort on developing flexible and novel training framework by combining other techniques with FL, including (1) Knowledge Distillation (KD), (2) Generative Adversarial Networks (GAN), (3) Neural Architecture Search (NAS), (4) Meta Learning, etc. Furthermore, we investigate the personalization in FL, which is also a good way to handle the above challenges.

