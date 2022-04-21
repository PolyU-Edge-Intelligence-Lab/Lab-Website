---
title: Radiation-free Spine Reconstruction and Posture Analysis Techniques with 3D Imaging
summary: Scoliosis is a sideways curvature of the spine that occurs most often during thegrowth spurt just before puberty. According to the survey and statistics of China Child Development Center, more than 20% teens have scoliosis.
tags:
- Smart Healthcare
date: "2022-03-27"

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
url_video: "https://www.youtube.com/watch?v=Cfx66gy9K9c"
---

Scoliosis is a sideways curvature of the spine that occurs most often during thegrowth spurt just before puberty. According to the survey and statistics of China Child Development Center, more than 20% teens have scoliosis. In addition to myopia and obesity, scoliosis has become the third biggest killer of youth health. According to some relevant survey data, 60% of teenagers have different degrees of posture problems. Early prevention and early treatment is the key of adolescent posture problems. Children who have mild scoliosis need to be monitored closely, usually with X-rays,to see if the curve is getting worse.

At present, the mainstream screening method is still manual detection, which has require patient naturally stands and bends at 90 degrees and the doctor makes a judgment based on the spinal line and morphological changes. However, such method has low efficiency and low accuracy and facing the severe shortage of physiotherapists. 

Meanwhile, during the COVID-19 epidemic, to help more people with rehabilitation needs realize remote screening and tracking and real-time AI monitoring of sports rehabilitation at home. A mobile-based posture screening algorithm and real-time exercise rehabilitation tracking algorithm are proposed.

In this project, we will design a 3D back image analysis method using commercial RGB-D to achieve low-cost, non-radiation, and sufficient accuracy of spine analysis and scoliosis screening. However, the analysis of the back image based on RGB-D is not simple and has the following three major challenges: (1) The back of the human body is an irregular curved surface, which is difficult to describe with some parametric models. (2) The point cloud image measured by commercial sensors is relatively sparse and has strong noise, and it is difficult to directly obtain the shape of the back. (3) The relationship between the back image and the spine shape is fuzzy.

{{< figure src="picture1.svg" caption="Hardware Design and Compoments" >}}

To address these challenges, we propose an automated all-in-one machine that performs comprehensive and accurate analysis, evaluation, and diagnosis of human posture: analysis items are in addition to common body dimensions. It also includes three-dimensional reconstruction of human spine based on infrared, foot pressure analysis, XO legs, pelvic deformation analysis and other functions; it is a set of comprehensive posture evaluation system with clinical significance in the real sense.

{{< figure src="picture2.svg" caption="Posture analysis algorithms" >}}

We also develop a Dr. Body APP, which uses AI algorithm to screen scoliosis, XO legs, high and low shoulders and other unhealthy postures through the photos of the back of the human body of the mobile phone for screening and severity classification; the use of a single photo of the human body for three-dimensional reconstruction of the human body for posture analysis and dimension measurement; Provide users with a variety of sports rehabilitation online courses, and record sports videos for intelligent action correction and analysis.

{{< figure src="picture3.svg" caption="App record user data and provide personalized follow-up service" >}}

**Innovation competition awards:** 

First Prize of Hong Kong University Student Innovation and Entrepreneurship Competition (2020); Hong Kong Social Enterprise Competition (HKSEC2019) Intellectual Property Ambassador Award; "Weining Cup" International AI Medical Challenge First Prize (2019), et.
