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
    opacity: 0;
    transition: opacity 1s ease-in-out;
  }

  .hero-fullscreen img.active {
    opacity: 1;
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
</style>

<div class="hero-fullscreen">
  <img src="/media/hello1.jpg" alt="Image 1" class="active">
  <img src="/media/hello2.jpg" alt="Image 2">
  <img src="/media/hello3.jpg" alt="Image 3">
  <!-- 添加更多图片 -->
</div>

<div id="dynamic-text">
  <!-- 动态文字将显示在这里 -->
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

  // 背景图片轮播
  const images = document.querySelectorAll('.hero-fullscreen img');
  let currentImageIndex = 0;

  function changeImage() {
    images[currentImageIndex].classList.remove('active');
    currentImageIndex = (currentImageIndex + 1) % images.length;
    images[currentImageIndex].classList.add('active');
  }

  setInterval(changeImage, 5000);  // 每5秒切换一次图片
</script>