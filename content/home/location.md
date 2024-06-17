---
widget: blank
headless: true
weight: 30

title: "LAB Location"
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

<!-- 引用 Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<div style="display: flex; align-items: center; font-size: 1.2em; margin-top: 20px;">
  <i class="fas fa-map-marker-alt" style="margin-right: 10px; color: #333;"></i>
  Room 326, Department of Computer Science, Chow Yei Ching Building, The University of Hong Kong, Pokfulam Road, Hong Kong
</div>
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
    var mymap = L.map('mapid').setView([22.33812,114.26439], 13);

    // 设置地图图层
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(mymap);

    // 添加标记
    var marker = L.marker([22.33812,114.26439]).addTo(mymap);
    marker.bindPopup("PEILab, HKUST").openPopup();
  };
  document.body.appendChild(script);
</script>
