---
title: (ICML2024)DiPrompT|Disentangled Prompt Tuning for Multiple Latent Domain Generalization in Federated Learning
summary: 

tags:
- Foundation Model
date: "2024-06-05"

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


Fine-tuning the learnable prompt for a pre-trained vision-language model (VLM), such as CLIP, has demonstrated exceptional efficiency in adapting to a broad range of downstream tasks. Existing prompt tuning methods for VLMs do not distinguish spurious features introduced by biased training data from invariant features, and employ a uniform alignment process when adapting to unseen target domains. This can impair the cross-modal feature alignment when the testing data significantly deviate from the distribution of the training data, resulting in a poor out-of-distribution (OOD) generalization performance. In this paper, we reveal that the prompt tuning failure in such OOD scenarios can be attribute to the undesired alignment between the textual and the spurious feature. As a solution, we propose CoOPood, a fine-grained prompt tuning method that can discern the causal features and deliberately align the text modality with the invariant feature. Specifically, we design two independent contrastive phases using two lightweight projection layers during the alignment, each with different objectives: 1) pulling the text embedding closer to invariant image embedding and 2) pushing text embedding away from spurious image embedding. We have illustrated that CoOPood can serve as a general framework for VLMs and can be seamlessly integrated with existing prompt tuning methods. Extensive experiments on various OOD datasets demonstrate the performance superiority over state-of-the-art methods.
