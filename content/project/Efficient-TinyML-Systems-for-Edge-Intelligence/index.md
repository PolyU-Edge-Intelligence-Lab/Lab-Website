---
title: Efficient TinyML Systems for Edge Intelligence
summary: In order to conquer the limitations of conventional in-cloud computing, it comes the rise of on-device learning, which makes the end-to-end ML procedure totally on user devices, without unnecessary involvement of the cloud.
tags:
- TinyML
date: "2016-10-27"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Type of Scoliosis 
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

Modern machine learning (ML) applications are often deployed in the cloud environment to exploit the computational power of clusters. However, this in-cloud computing scheme cannot satisfy the demands of emerging edge intelligence scenarios, including providing personalized models, protecting user privacy, adapting to real-time tasks and saving resource cost. In order to conquer the limitations of conventional in-cloud computing, it comes the rise of on-device learning, which makes the end-to-end ML procedure totally on user devices, without unnecessary involvement of the cloud. In spite of the promising advantages of on-device learning, implementing a high-performance on-device learning system still faces with many severe challenges, such as insufficient user training data, backward propagation blocking and limited peak processing speed.

## Objectives

Observing the substantial improvement space in the implementation and acceleration of on-device learning systems, our group devote to designing high-performance TinyML architectures and relevant optimization algorithms, especially for embedded devices and microprocessors. Our research focuses on the software and hardware synergy of on-device learning techniques, covering the scope of model-level neural network design, algorithm-level training optimization and hardware-level instruction acceleration.

## Achievements

The on-device learning techniques can be employed in many emerging TinyML scenarios, where the system performance if often bounded by the limited hardware resources. Currently, our group have achieved breakthroughs on improving the computational capacity and designing domain-specific AI chips for task acceleration. These chips can be designed from the perspectives of model compression, few-shot learning, quantization-ware training, memory management and the low-level instructions. We pursue the vision that helps researchers and developers optimize AI deployment without tedious code modifications. Some research demos have been open-source on Github, please visit at:
- {{< icon name="github-square" pack="fab" >}}[https://github.com/kimihe](https://github.com/kimihe)
- {{< icon name="github-square" pack="fab" >}}[https://github.com/FromSystem](https://github.com/FromSystem)

## Cooperators

Our group have established close cooperation with industrial communities, including Alibaba, Huawei, Nvidia, Webank, Tencent, etc.

## PhD/intern Applications

We are looking for students and partners who are interested in:
- On-device/TinyML Systems (for Edge Intelligence)
- Distributed Machine Learning Systems (for Data center)
- Modern AI/ML frameworks, e.g., NVIDIA NCCL, CUDA, TensorRT, Apple CoreML, PyTorch, TensorFlow, Keras, BytePS, Gym, etc.
- Domain-specific hardware optimization and implementation, e.g., NVIDA Jetson, FPGA, Microprocessors, AI Chips, etc.
- Coding contribution to our GitHub repositories