1. background系列
   1.1 background-image
      ① url()

   1.1 ②两个background-image属性--使用逗号连接
   background-image: linear-gradient(
        to right bottom, 
        rgba(126, 213, 111, 0.8), 
        rgba(40, 180, 131, 0.8)), 
    url(../image/hero.jpg);
    上层是渐变色，下层是图片

   1.2 background-position
   1.3 background-size

2. clip-path裁剪

3. h1是页面上最重要的标题，对搜索引擎很重要。可以通过span分隔的方式，设置语义连贯但样式不同的文字


布局技巧：
1.img是行内元素，常在其外包裹一个div，便于布局;alt属性利于SEO（Search Engine Optimization搜索引擎优化)，也用于图片无法加载的情况

2.使用absolute定位和transform配合，使元素垂直水平居中