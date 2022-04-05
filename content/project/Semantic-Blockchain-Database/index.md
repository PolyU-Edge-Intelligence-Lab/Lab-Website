---
title: 	Semantic Query and Index Layer in Semantic Blockchain Database
summary: Blockchain database is a new direction that constructs index on top of blockchain to provide rich query functionalities. The existing works are either insecure because the query process separates from the blockchain consensus, or inscalable because all the data needs to be stored in the block. Therefore, we propose an authenticated semantic database layer for blockchains.
tags:
- Blockchain
date: "2022-03-18"

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

## Background

Blockchain database is a new direction that constructs index on top of blockchain to provide rich query functionalities. The existing works are either insecure because the query process separates from the blockchain consensus, or inscalable because all the data needs to be stored in the block. Therefore, we propose an authenticated semantic database layer for blockchains. We design a hybrid on/off chain blockchain storage architecture in which the majority of blockchain storage is offloaded to the off-chain storage and a novel index structure named Merkle Semantic Trie (MST) is designed to be a secure and semantic bridge between on- and off-chain. Based on MST, MSTDB provides a variety of semantic query functions including multi-keyword query, range query, Top-K query, and cross-chain query. Besides, to improve the performance further, we design some index compression and query preprocessing techniques for our semantic database layer.

## Reference

An Efficient Query Scheme for Hybrid Storage Blockchains based on Merkle Semantic Trie, Best Paper Award Runner Up received in SRDS 2020 (CCF-B).

