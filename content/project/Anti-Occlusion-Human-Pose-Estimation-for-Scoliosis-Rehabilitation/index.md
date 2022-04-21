---
title: Anti-Occlusion Human Pose Estimation for Scoliosis Rehabilitation
tags:
- Smart Healthcare
date: "2022-01-01"

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

Physiotherapeutic scoliosis-specific exercises (PSSE) have been proved to be effective in scoliosis rehabilitation. PSSE consist of a program of curve-specific exercise protocols which are individually adapted to a patients’ curve site, magnitude, and clinical characteristics. Specific PSSE are used to help relieve scoliosis symptoms. PSSE is not generalized physiotherapy exercises which are generic exercises usually consisting of low impact stretching and strengthening activities like yoga, Pilates and the Alexander technique but especially designed exercise for scoliosis patients that requires professional guidance. Wrong movement may cause severe damage to the spine again.

During the COVID-19 pandemic, Exercise at specific medical centres with crowd around is risky. Smart phone, however, is now prevalence all over the world. Almost every smart phone contains at least one 2D camera that can capture video stream. If we can use this device to track patients’ movement, it may be way more convenient for doctors to guide the patients remotely.

Human pose estimation is one of the best matches of tracking patient movement at home.

Recent years have witnessed learning-based human pose estimation getting popular in more scenarios with occlusions, where invisible areas for perception objects significantly affect accuracy. Existing methods mainly use convolutional neural networks as the backbone and get limited local features to recover the occluded part. Such an anti-occlusion pipeline often suffers from the challenges of self-occlusion scenery, where similar parts of occluders and occludees are ambiguous. In this case, we need to design a masked visual autoencoder for image processing and video streaming, which recovers occluded regions by extracting deep spatial information at a higher semantic level. This autoencoder can get better details inferred from global self-attention and thus improves accuracy. The gist is to train the autoencoder to extract key-point information from the joint tokens that are manually masked in a self-supervised manner to simulate the occlusion in video streaming. To use dataset more efficiently and extract more information from a single image, we generate several different positive samples simulating more occluded cases by randomly mask more patches in joint tokens. We also propose an end-to-end pipeline for training and inference, which can effectively reduce the dependency of annotated occluded datasets and can be further applied to other visual tasks. This pipeline can obtain a great computation saving with much fewer annotated datasets and hold a higher runtime performance over the SOTA ViT methods.
