---
widget: hero
headless: true
active: true
weight: 1

title: ""
subtitle: ""
# hero_media: "hello1.jpg" 

design:
  background:
    image: "hello1.jpg"
    image_darken: 0.6
    image_parallax: true
    image_position: center
    image_size: cover
    text_color_light: true

---

<style>
  .hero-fullscreen {
    position: relative;
    height: 100vh;
    width: 100%;
    overflow: hidden;
  }

  .hero-fullscreen img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  #dynamic-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 2em;
    color: white;
    text-align: center;
  }

  #scroll-down {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 2em;
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

<div class="hero-fullscreen">
  <img src="/media/hello1.jpg" alt="Background Image">
</div>

<div id="dynamic-text">
  <!-- 动态文字将显示在这里 -->
</div>

<div id="scroll-down">
  &#x25BC;
</div>

<script>
  const texts = ["Welcome to Pervasive Intelligence Lab 👋", "Join Us on Our Journey"];
  let count = 0;
  let index = 0;
  let currentText = '';
  let letter = '';

  (function type(){
    if (count === texts.length) {
      count = 0;
    }
    currentText = texts[count];
    letter = currentText.slice(0, ++index);

    document.getElementById('dynamic-text').textContent = letter;
    if (letter.length === currentText.length) {
      count++;
      index = 0;
      setTimeout(type, 2000);  // 2秒后切换到下一个文本
    } else {
      setTimeout(type, 50);  // 每50ms显示一个新字母
    }
  }());

  // 滚动到下一部分
  document.getElementById('scroll-down').addEventListener('click', function () {
    window.scrollTo({
      top: window.innerHeight,
      behavior: 'smooth'
    });
  });
</script>