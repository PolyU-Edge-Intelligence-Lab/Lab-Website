---
widget: blank
headless: true
weight: 5

title: ""
subtitle: ""

design:
  columns: '1'
  # background:
  #   image: 
  #   image_darken: 0
  #   image_size: cover
  #   image_position: right
  #   image_parallax: true
  #   text_color_light: false
  #   text_position: 
# advanced:
#   css_style:
#   css_class: 

---

The Pervasive Intelligence Laboratory, directed by [Prof. Song Guo](https://cse.hkust.edu.hk/admin/people/faculty/profile/songguo), is developing novel and efficient deep learning architectures, algorithms, and systems over ubiquitous mobile, IoT, and edge endpoints. By pushing the boundaries of AI capabilities, we aim to unlock new possibilities and create significant impacts in multiple areas such as scientific discovery, environmental sustainability, and societal well-being.

We focus on the following research areas:

<!-- - **Cloud-Edge Collaborative Large Models:** We focus on building open, intelligent, and efficient AI large models that cater to the diverse data and resources distributed across edge endpoints. Our goal is to satisfy the multi-faceted demands of large model training, fine-tuning, inference, and deployment, while optimizing the model construction process through intelligent means to enhance performance. We aim to drive the widespread adoption of AIGC in vertical application scenarios, achieving deep technology integration and maximum value creation.
- **AI Computing Cyberinfrastructure:** We are building a federated edge intelligence platform tailored for large models, leveraging our 'algorithm-network-intelligence' integrated technology to design algorithms that adapt large models to edge environments based on 'hybrid expert models'. By harnessing edge computing network technology, we integrate fragmented computing resources at the edge, enabling large models to run on edge devices and supporting various generative AI capabilities. This will reduce hardware costs and expand the spatiotemporal scope of large model services.
- **Trustworthy AI Governance:** As large models are increasingly deployed, their security concerns are becoming more pronounced. We are committed to researching the security challenges faced by large models, including data poisoning and adversarial attacks, with the goal of building secure, trustworthy, and robust AI models that promote the development of trustworthy AI governance.
- **AI4Science:** AI technology has made breakthroughs in challenging tasks such as weather forecasting. We focus on training and developing ultra-high-resolution meteorological large models driven by data, as well as researching AI assimilation algorithms and extreme disaster prediction (e.g., FengWu-GHR), contributing to the advancement of scientific research. -->

- **Cloud-Edge Collaborative Large Models**
- **AI Computing Cyberinfrastructure**
- **Trustworthy AI Governance & AIGC**
- **AI4Science**
  

  
## Join Us

We are looking for strongly motivated PhD students, Research Assistants, and Postdoctoral Fellows.

[{{< icon name="envelope" pack="fas" >}}Song Guo](mailto:songguo@cse.ust.hk)

<script type="text/javascript" src="static/js/leaflet.js"></script>
<link rel="stylesheet" href="static/css/leaflet.css"/>

<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators">
    <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="home/homepage.jpg" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="home/birthday.jpg" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="home/hiking.jpg" alt="Third slide">
    </div>
  </div>
  <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

---
LAB Location
---

<div id="mapid" style="width: 100%; height: 400px;"></div>

<script>
  // 加载 Leaflet.js 库
  var link = document.createElement("link");
  link.rel = "stylesheet";
  link.href = "https://unpkg.com/leaflet@1.7.1/dist/leaflet.css";
  document.head.appendChild(link);

  var script = document.createElement("script");
  script.src = "https://unpkg.com/leaflet@1.7.1/dist/leaflet.js";
  script.onload = function() {
    // 初始化地图
    var mymap = L.map('mapid').setView([114.2,22.3], 13);

    // 设置地图图层
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(mymap);

    // 添加标记
    var marker = L.marker([114.2,22.3]).addTo(mymap);
    marker.bindPopup("<b>Hello world!</b><br>I am a popup.").openPopup();
  };
  document.body.appendChild(script);
</script>
---
