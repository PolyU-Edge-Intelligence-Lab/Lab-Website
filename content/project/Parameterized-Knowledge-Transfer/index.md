---
title: Heterogeneous Hardware \& Data- Parameterized Knowledge Transfer
summary: Most existing pFL methods rely on model parameters aggregation at the server side, which require all models to have the same structure and size. Such constraints would prevent status quo pFL methods from further application in practical scenarios, where clients are often willing to own unique models, i.e., with customized neural architectures to adapt to heterogeneous capacities in computation, communication and storage space, etc. We seek to develop a novel training framework that can accommodate heterogeneous model structures for each client and achieve personalized knowledge transfer in each FL training round. 

tags:
- Federated Learning
date: "2022-03-17"

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

Most existing pFL methods rely on model parameters aggregation at the server side, which require all models to have the same structure and size. Such constraints would prevent status quo pFL methods from further application in practical scenarios, where clients are often willing to own unique models, i.e., with customized neural architectures to adapt to heterogeneous capacities in computation, communication and storage space, etc. We seek to develop a novel training framework that can accommodate heterogeneous model structures for each client and achieve personalized knowledge transfer in each FL training round. Specifically, the aggregation procedure in original pFL is formulated into a personalized group knowledge transfer training algorithm, which enable each client to maintain a personalized soft prediction at the server side to guide the others' local training.

<!-- {{< figure src="parameterized- knowledge-transfer-2.png" caption="Our work: Parameterized Knowledge Transfer for Personalized Federated Learning [5]." >}} -->

##### Reference:

[5]. Parameterized Knowledge Transfer for Personalized Federated Learning. *NeurIPS*, <u>CCF-A</u>