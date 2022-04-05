---
title: Edge Application Layer in Blockchain-empowered Edge Learning
summary: Blockchain-empowered edge learning is a novel distributed learning architecture to dispense with a dedicated server in traditional distributed learning and provide trustworthy training for edge devices.
tags:
- Blockchain
date: "2022-03-20"

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

Blockchain-empowered edge learning is a novel distributed learning architecture to dispense with a dedicated server in traditional distributed learning and provide trustworthy training for edge devices. It is based on a blockchain platform in which the edge devices for distributed learning participate in the consensus and commit and receive transactions about the learning process including edge data collection, edge model weights, training results, etc. However, existing blockchains cannot be directly used for swarm learning because their consensus protocols often commit transactions in blocks, each of which requires minutes, while swarm learning produces massive data about the learning processes in real-time. Moreover, the edge devices are often unable to meet the hardware requirement of the existing blockchain consensus such as the computation-intensive mining in Proof-of-Work (PoW). Therefore, we are going to design a streaming blockchain system and smart contract engine for swarm learning.
