---
title: Efficient Federated Learning Framework for Heterogeneous Environment
summary: Federated learning (FL) has been proposed as a promising solution for future AI applications with strong privacy protection. It enables distributed computing nodes to collaboratively train models without exposing their own data. 

tags:
- Federated Learning
date: "2022-04-01"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Research Overview of the Federated Learning Paradigm
  focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
# url_code: ""
# url_png: ""
# url_slides: ""
# url_video: ""
---

## Research Overview

{{< figure src="featured.png" caption="Research Overview of the Federated Learning Paradigm" >}}

Our team aims to design promising solutions for future AI applications in Federated Learning (FL) systems, which enable distributed computing nodes to collaboratively train machine learning models without exposing their own data. We focus on solving the following challenging issues:

* Heterogeneous Hardware & Data
* Resource constraints
* Expensive communication
* Lack of participants

##### Reference:

[1]. Edge Learning: the Enabling Technology for Distributed Big Data Analytics in the Edge. *ACM Computing Surveys (TC)*, <u>JCR-Q1</u>

[2]. A Survey of Incentive Mechanism Design for Federated Learning. *IEEE Transactions on Emerging Topics in Computational Intelligence (TETCI)*, <u>JCR-Q1</u>

In the following, we will explain the related technologies:

### **Heterogeneous Data & Resource Constraints: Batch Size Adaptation**

{{< figure src="batch-szie-adaptation-1.png" caption="Heterogeneous Data" >}}

**Introduction**: Federated learning (FL) has been widely recognized as a promising approach by enabling individual participants to cooperatively train a global model without exposing their own data. One of the key challenges in FL is that data distributions in different participants are usually non-independently and identically distributed (non-IID). For example, different areas can have very different disease distributions. Besides, the participants are usually resource-constrained with limited computational power, storage capacity, transmission range and battery. It is essential to design novel training framework to address above challenges. However, existing approaches either consider the optimization of server-side aggregation or focus on improving the client-side training efficiency, which only lead to sub-optimal performance. Therefore, we are going to investigate a new method to improve training efficiency of each client from the perspective of whole training process under the circumstances of non-IID data. In our proposed framework, both the local training and global aggregation are optimized by using a deep reinforcement learning agent to determine the batch size of each client according to the current state in each communication round.

{{< figure src="batch-szie-adaptation-2.png" caption="Workflow of the proposed batch Size Adaptation [3]." >}}

##### Reference:

[3]. Adaptive Federated Learning on Non-IID Data with Resource Constraint. *IEEE Transactions on Computers (TC)*, <u>CCF-A</u>

### **Heterogeneous Data & Expensive Communication: Layer-wised Aggregation**

**Introduction**: Instead of collaboratively train only one global for all clients, personalized federated learning (pFL) mechanisms are proposed to allow each client to train a customized model to adapt to their own data distribution. Researches over the past few years have applied the weighted aggregation manner to produce personalized models, where the weights are determined by calibrating the distance of the entire model parameters or loss values, and have yet to consider the layer-level impacts to the aggregation process, leading to lagged model convergence and inadequate personalization over non-IID datasets. We design a novel pFL training framework dubbed Layer-wised Personalized Federated learning (pFedLA) that can discern the importance of each layer from different clients, and thus is able to optimize the personalized model aggregation for clients with heterogeneous data. 

{{< figure src="Layer-wised-Aggregation.png" caption="Workflow of the Layer-wised aggregation method [4]. We use hypernetwork to identify the mutual contribution factors at layer granularity." >}}

##### Reference:

[4]. Layer-wised Model Aggregation for Personalized Federated Learning. *CVPR*, <u>CCF-A</u>

### **Heterogeneous Hardware & Data: Parameterized Knowledge Transfer**

{{< figure src="parameterized- knowledge-transfer-1.png" caption="Heterogeneous Model & Expensive Communication overhead (i.e., 10-class classification)" >}}

**Introduction**: Most existing pFL methods rely on model parameters aggregation at the server side, which require all models to have the same structure and size. Such constraints would prevent status quo pFL methods from further application in practical scenarios, where clients are often willing to own unique models, i.e., with customized neural architectures to adapt to heterogeneous capacities in computation, communication and storage space, etc. We seek to develop a novel training framework that can accommodate heterogeneous model structures for each client and achieve personalized knowledge transfer in each FL training round. Specifically, the aggregation procedure in original pFL is formulated into a personalized group knowledge transfer training algorithm, which enable each client to maintain a personalized soft prediction at the server side to guide the others' local training.

{{< figure src="parameterized- knowledge-transfer-2.png" caption="Our work: Parameterized Knowledge Transfer for Personalized Federated Learning [5]." >}}

##### Reference:

[5]. Parameterized Knowledge Transfer for Personalized Federated Learning. *NeurIPS*, <u>CCF-A</u>

### **Lack of participants: Incentive Mechanism Design for Federated Learning**

{{< figure src="incentive-1.png" caption="Incentive metrics" >}}

**Introduction**: The main objective of incentive is to motive data owners to participate in FL. A few of works have designed incentive mechanisms for FL, but these mechanisms only consider myopia optimization on resource consumption, which results in the lack of learning algorithm performance guarantee and long-term sustainability. We propose Chiron, an incentive-driven long-term mechanism for edge learning based on hierarchical deep reinforcement learning. First, our optimization goal combines learning-algorithms metric (i.e., model accuracy) with system metric (i.e., learning time, and resource consumption), which can improve edge learning quality under a fixed training budget. Second, we present a two-layer H-DRL design with exterior and inner agents to achieve both long-term and short-term optimization for edge learning, respectively.

{{< figure src="incentive-2.png" caption="Our work: Hierarchical Reinforcement Learning for Incentive mechanism in Federated Learning [6]." >}}

##### Reference:

[6]. Incentive-Driven Long-term Optimization for Edge Learning by Hierarchical Reinforcement Mechanism. *ICDCS*, <u>CCF-B</u>