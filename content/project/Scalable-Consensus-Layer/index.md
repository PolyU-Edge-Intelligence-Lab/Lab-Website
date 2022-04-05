---
title: Layered Sharding Architecture for Blockchain
summary: Most existing blockchain systems adopt a static policy that cannot efciently deal with the dynamic environment in the blockchain system, i.e., joining and leaving of nodes, and malicious attack. Therefore, we propose a novel dynamic sharding-based blockchain framework to achieve a good balance between performance and security without compromising scalability under a dynamic environment.
tags:
- Blockchain
date: "2022-03-14"

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

## Introduction

As a promising solution to blockchain scalability, sharding divides blockchain nodes into small groups called shards, splitting the workload. Existing works for sharding, however, are limited by cross-shard transactions, since they need to split each cross-shard transaction into multiple sub-transactions, each of which costs a consensus round to commit. To deal with the serious performance degradation brought by cross-shard transactions. Therefore, we propose a novel layered sharding architecture for blockchain and a cooperation-based layered sharding consensus. The basic idea is to allow shards to overlap, rather than isolating them completely, so that some nodes can locate in more than one shard. For cross-shard transactions, nodes located in the overlap of these shards can cooperative to verify, process and commit them directly and efficiently.

## Reference

 Pyramid: A Layered Sharding Blockchain System, INFOCOM 2021 (CCF-A).

