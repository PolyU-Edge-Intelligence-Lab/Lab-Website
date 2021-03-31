---
title: New Architectures and Methodologies for High Performance Sharding Blockchain
summary: Blockchain draws tremendous attention from academia and industry, since it can provide distributed ledgers with data transparency, integrity, and immutability to untrusted parties for various decentralized applications.
tags:
- Blockchain
date: "2016-04-27"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Blockchain Sharding 
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

Blockchain draws tremendous attention from academia and industry, since it can provide distributed ledgers with data transparency, integrity, and immutability to untrusted parties for various decentralized applications. However, it is still challenging for blockchain to deal with large-scale networks because of the limited scalability of the blockchain systems. Sharding is a novel blockchain architecture that is proved to significantly improve the scalability of blockchain. Its main idea is to divide blockchain nodes into small groups called shards, which can handle transactions in parallel. To exploit the shortages of blockchain sharding for real application environment, we conduct two research projects as follows.

First, to deal with the serious performance degradation brought by cross-shard transactions, we propose a novel layered sharding architecture for blockchain and a cooperation-based layered sharding consensus. The basic idea is to allow shards to overlap, rather than isolating them completely, so that some nodes can locate in more than one shard. For cross-shard transactions, nodes located in the overlap of these shards can cooperative to verify, process and commit them directly and efficiently.

{{< figure src="picture1.svg" caption="Blockchain and Training" >}}

Second, most existing blockchain sharding systems adopt a static sharding policy that cannot efciently deal with the dynamic environment in the blockchain system, i.e., joining and leaving of nodes, and malicious attack. We propose a novel dynamic sharding-based blockchain framework to achieve a good balance between performance and security without compromising scalability under a dynamic environment. For the framework, a deep reinforcement learning (DRL)-based consensus is designed to acquire optimal sharding policies in a series of dynamic and high-dimensional environment states.
