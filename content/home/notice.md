---
widget: hero
headless: true
active: true
weight: 1

title: ""
subtitle: ""

design:
  background:
    image_darken: 0.6
    image_parallax: true
    text_color_light: true
advanced:
  css_style: |
    .background-container {
      position: relative;
      height: 40vh; /* 设置背景图片高度为视口高度的40% */
      overflow: hidden;
    }

    .background-container img {
      position: absolute;
      width: 100%;
      height: 100%;
      object-fit: cover;
      animation: slide 15s infinite; /* 背景图滚动播放动画 */
    }

    @keyframes slide {
      0% { opacity: 1; }
      33% { opacity: 0; }
      66% { opacity: 0; }
      100% { opacity: 1; }
    }

    .background-container img:nth-child(1) {
      animation-delay: 0s;
    }

    .background-container img:nth-child(2) {
      animation-delay: 5s;
    }

    .background-container img:nth-child(3) {
      animation-delay: 10s;
    }

    #dynamic-text-top {
      position: absolute;
      top: 20%; /* 调整文本位置以适应新的背景高度 */
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 4vh; /* 使用视口宽度单位 */
      color: white;
      text-align: center;
    }

    #dynamic-text-bottom {
      position: absolute;
      top: 85%; /* 调整文本位置以适应新的背景高度 */
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 2vh; /* 使用视口宽度单位 */
      color: white;
      text-align: center;
    }

    #scroll-down {
      position: absolute;
      bottom: 10px;
      left: 50%;
      transform: translateX(-50%);
      font-size: 3.5vh; /* 使用视口宽度单位 */
      color: white;
      text-align: center;
      cursor: pointer;
      animation: bounce 2s infinite;
    }

    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% {
        transform: translateY(0);
      }
      40% {
        transform: translateY(-10px);
      }
      60% {
        transform: translateY(-5px);
      }
    }
  css_class:
---

<div class="background-container">
  <img src="image1.png" alt="Background Image 1">
  <img src="image2.png" alt="Background Image 2">
  <img src="image3.png" alt="Background Image 3">
</div>

<div id="dynamic-text-top"></div>
<div id="dynamic-text-bottom"></div>
<div id="scroll-down">&#x25BC;</div>

<script>
  const textsTop = ["Welcome to Pervasive Intelligence Lab (PEILab) 👋"];
  const textsBottom = ["Join Us on Our Journey in HKUST"];
  function typeText(elementId, texts, callback) {
    let count = 0;
    let index = 0;
    let currentText = '';
    let letter = '';
    (function type(){
      if (count === texts.length) {
        if (callback) callback();
        return;
      }
      currentText = texts[count];
      letter = currentText.slice(0, ++index);
      document.getElementById(elementId).textContent = letter;
      if (letter.length === currentText.length) {
        count++;
        index = 0;
        setTimeout(type, 1000);
      } else {
        setTimeout(type, 30);
      }
    }());
  }
  typeText('dynamic-text-top', textsTop, function() {
    typeText('dynamic-text-bottom', textsBottom);
  });
  document.getElementById('scroll-down').addEventListener('click', function () {
    window.scrollTo({
      top: window.innerHeight,
      behavior: 'smooth'
    });
  });
</script>