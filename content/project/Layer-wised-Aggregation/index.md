---
title: Heterogeneous Data \& Expensive Communication- Layer-wised Aggregation
summary: We design a novel pFL training framework dubbed Layer-wised Personalized Federated learning (pFedLA) that can discern the importance of each layer from different clients, and thus is able to optimize the personalized model aggregation for clients with heterogeneous data. 

tags:
- Federated Learning
date: "2022-03-19"

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

Instead of collaboratively train only one global for all clients, personalized federated learning (pFL) mechanisms are proposed to allow each client to train a customized model to adapt to their own data distribution. Researches over the past few years have applied the weighted aggregation manner to produce personalized models, where the weights are determined by calibrating the distance of the entire model parameters or loss values, and have yet to consider the layer-level impacts to the aggregation process, leading to lagged model convergence and inadequate personalization over non-IID datasets. We design a novel pFL training framework dubbed Layer-wised Personalized Federated learning (pFedLA) that can discern the importance of each layer from different clients, and thus is able to optimize the personalized model aggregation for clients with heterogeneous data. 

<!-- {{< figure src="Layer-wised-Aggregation.png" caption="Workflow of the Layer-wised aggregation method [4]. We use hypernetwork to identify the mutual contribution factors at layer granularity." >}} -->

##### Reference:

[4]. Layer-wised Model Aggregation for Personalized Federated Learning. *CVPR*, <u>CCF-A</u>