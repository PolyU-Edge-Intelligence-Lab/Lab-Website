---
# An instance of the Pages widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: pages

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 15

title: Recent Publications
subtitle: ''

content:
  # Page type to display. E.g. post, talk, publication...
  page_type: publication
  # Choose how much pages you would like to display (0 = all pages)
  count: 5
  # Choose how many pages you would like to offset by
  offset: 0
  # Page order: descending (desc) or ascending (asc) date.
  order: desc
  # Filter on criteria
  filters:
    tag: ''
    category: ''
    publication_type: ''
    author: ''
    exclude_featured: false
design:
  # Choose a view for the listings:
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   4 = Citation (publication only)
  view: 4
  columns: "1"
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

---
