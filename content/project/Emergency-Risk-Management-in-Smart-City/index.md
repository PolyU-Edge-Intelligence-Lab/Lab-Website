---
title: Emergency Risk Management in Smart City
summary: With the emergence and drastic improvement of mobile devices (e.g., phones, tablets, drones, and autonomous vehicles), we are now witnessing an exciting revolution of the digital city.
tags:
- Smart City
date: "2016-08-27"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 'Transform Cities with Smart Technology'
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

With the emergence and drastic improvement of mobile devices (e.g., phones, tablets, drones, and autonomous vehicles), we are now witnessing an exciting revolution of the digital city. Specifically, with the popularity of 5G networks, video-sharing and live-streaming applications (e.g., TikTok, BIGO, and Twitch) are becoming increasingly widespread. Besides allowing individuals to share life experiences and moments with their followers, video-based applications could also be a promising tool for sensing complex and dynamic urban environments.

With the development of AI-empowered video processing techniques, the ubiquitous mobile camera network has the potential to go beyond the video-surveillance system to capture various risks in the complex and dynamic city environment. However, the edge device has limited computation resource compared to the desktop GPU and CPU, which brings new challenge for optimizing AI algorithm for executing on edge devices. 

{{< figure src="picture1.jpg" caption="Resource-constraint Mobile Devices" >}}

Another major challenge is the heterogeneous of edge hardware. The AI models need to adapt to heterogeneous edge devices with significant ram and computation difference. The last challenge is view limitation. Since each edge device usually has a small field of view, it is very hard to capture an integrated scenario in the smart city. To support practical real-time risk detection, we must joint use multiple cameras to obtain abundant regional data.

{{< figure src="picture2.png" caption="Heterogeneous Mobile Devices" >}}