---
widget: hero
headless: true
active: true
weight: 1

title: ""
subtitle: ""

design:
  background:
    image: "Redbird.png"
    image_darken: 0.6
    image_parallax: true
    image_position: center
    image_size: cover
    text_color_light: true
advanced:
  css_style:
  css_class:
---
<style>
  #background-container {
    position: relative;
    width: 100%;
    height: 25vh; /* 设置背景图高度为视口高度的40% */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    overflow: hidden;
  }

  #background-container::before {
    content: "";
    background: url('Redbird.png') center center / cover no-repeat;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0.6; /* 设置背景图的透明度 */
  }

  #dynamic-text-top {
    position: absolute;
    top: 40%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 2vh; /* 使用视口宽度单位 */
    color: white;
    text-align: center;
    white-space: nowrap;
  }

  #dynamic-text-bottom {
    position: absolute;
    top: 90%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 1vh; /* 使用视口宽度单位 */
    color: white;
    text-align: center;
  }

  #scroll-down {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 1vh; /* 使用视口宽度单位 */
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
</style>
<div id="background-container">
  <div id="dynamic-text-top"></div>
  <div id="dynamic-text-bottom"></div>
  <div id="scroll-down">&#x25BC;</div>
</div>
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