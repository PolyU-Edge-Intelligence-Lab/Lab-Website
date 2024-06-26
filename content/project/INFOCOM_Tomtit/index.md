---
title: "(INFOCOM2024)Tomtit:Hierarchical Federated Fine-Tuning of Giant Models based on Autonomous Synchronization"

tags:
- Foundation Model
date: "2023-09-22"


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
#url_video: "https://www.youtube.com/watch?v=Cfx66gy9K9c"
---

With the rapid advancement of giant models, the paradigm of pre-training models followed by fine-tuning for specific downstream tasks has become increasingly popular. In response to the challenges faced by adapter-based fine-tuning due to insufficient data, and the scalability and inflexibility issues of existing federated fine-tuning solutions, we introduce Tomtit. Tomtit is a hierarchical federated fine-tuning system designed to significantly accelerate the fine-tuning process and enhance the energy efficiency of devices.

Tomtit's core innovation lies in its distributed design, which allows each edge and device to adopt a unique synchronization scheme tailored to their specific heterogeneity in model structure, data distribution, and computing capability. Through extensive empirical studies, we have discovered that model synchronization schemes—specifically, the timing of synchronizing models between edges and devices—are crucial in federated fine-tuning.

Moreover, Tomtit comes with a theoretical guarantee of convergence, ensuring its robustness and reliability. We have developed a prototype of Tomtit and conducted evaluations on a testbed. Experimental results demonstrate that Tomtit significantly outperforms the current state-of-the-art solutions.


More information refer to Tomtit: Hierarchical Federated Fine-Tuning of Giant Models based on Autonomous Synchronization, INFOCOM 2024.
