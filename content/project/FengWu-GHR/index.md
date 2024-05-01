---
title: FengWu-GHR | Learning the Kilometer-scale Medium-range Global Weather Forecasting
tags:
- Ai for Science
date: "2024-01-28"


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

FengWu-GHR: Learning the Kilometer-scale Medium-range Global Weather Forecasting The first data-driven global weather forecasting model running at the 0.09◦ horizontal resolution. FengWu-GHR introduces a novel approach that opens the door for operating ML-based high-resolution forecasts by inheriting prior knowledge from a pretrained low-resolution model. The hindcast of weather prediction in 2022 indicates that FengWu-GHR is superior to the IFS-HRES. Furthermore, evaluations on station observations and case studies of extreme events support the competitive operational forecasting skill of FengWu-GHR at the high resolution.

## Prototype Overview 

Kilometer-scale modeling of global atmosphere dynamics enables fine-grained weather forecasting and decreases the risk of disastrous weather and climate activity. Therefore, building a kilometer-scale global forecast model is a persistent pursuit in the meteorology domain. Active international efforts have been made in past decades to improve the spatial resolution of numerical weather models. Nonetheless, developing the higher resolution numerical model remains a long-standing challenge due to the substantial consumption of computational resources. Recent advances in data-driven global weather forecasting models utilize reanalysis data for model training and have demonstrated comparable or even higher forecasting skills than numerical models. However, they are all limited by the resolution of reanalysis data and incapable of generating higherresolution forecasts. This work presents FengWu-GHR, the first data-driven global weather forecasting model running at the 0.09◦ horizontal resolution. FengWu-GHR introduces a novel approach that opens the door for operating MLbased high-resolution forecasts by inheriting prior knowledge from a pretrained low-resolution model. The hindcast of weather prediction in 2022 indicates that FengWu-GHR is superior to the IFS-HRES. Furthermore, evaluations on station  observations and case studies of extreme events support the competitive operational forecasting skill of FengWu-GHR at the high resolution.


{{< figure src="1.png" caption="" >}}
