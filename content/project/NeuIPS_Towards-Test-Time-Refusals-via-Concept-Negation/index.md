---
title: (NeurIPS2023) Towards Test-Time Refusals via Concept Negation
tags:
- Trustworthy AI
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

PROTORE works by incorporating CLIP’s language-contrastive knowledge to identify the prototype of negative concepts, extract the negative features from outputs using the prototype as a prompt, and further refine the attention maps by retrieving negative features.

## Prototype Overview

Generative models produce unbounded outputs, necessitating the use of refusal techniques to confine their output space. Employing generative refusals is crucial in upholding the ethical and copyright integrity of synthesized content, particularly when working with widely adopted diffusion models. Concept negation” presents a promising paradigm to achieve generative refusals, as it effectively defines and governs the model’s output space based on oncepts, utilizing natural language interfaces that are readily comprehensible to humans. However, despite the valuable contributions of prior research to the field of concept negation, it still suffers from significant limitations. The existing concept negation methods, which operate based on the composition of score or noise predictions from the diffusion process, are limited to independent concepts (e.g., “a blonde girl” without “glasses”) and fail to consider the interconnected nature of concepts in reality (e.g., “Mickey mouse eats ice cream” without “Disney characters”). Keeping the limitations in mind, we propose a novel framework, called PROTORE, to improve the flexibility of concept negation via test-time negative concept identification along with purification in the feature space. PROTORE works by incorporating CLIP’s language-contrastive knowledge to identify the prototype of negative concepts, extract the negative features from outputs using the prototype as a prompt, and further refine the attention maps by retrieving negative features. Our evaluation on multiple benchmarks shows that PROTORE outperforms state-of-the-art methods under various settings, in terms of the effectiveness of purification and the fidelity of generative images.

{{< figure src="1.png" caption="" >}}