---
title: "Welcome"
subtitle: ""
type: "widget_page"
---

# Hero widget
---
widget: hero
headless: true
active: true
weight: 1

title: "Hi, I am John"
subtitle: ""
hero_media: "hello1.jpg"  # 将此处替换为你想要显示的大图的文件名

design:
  background:
    image: "hello1.jpg"  # 确保图像文件存在于 `static/media/` 目录下
    image_darken: 0.6
    image_parallax: true
    image_position: center
    image_size: cover
    text_color_light: true
---

# HTML widget for dynamic text
---
widget: blank
headless: true
active: true
weight: 15

design:
  columns: "1"

html: |
  <div id="dynamic-text" style="font-size: 2em; color: white; text-align: center;">
    <!-- 动态文字将显示在这里 -->
  </div>

  <script>
    const texts = ["Welcome to My Lab", "We Explore Science", "Join Us on Our Journey"];
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
        setTimeout(type, 200);  // 每200ms显示一个新字母
      }
    }());
  </script>
---