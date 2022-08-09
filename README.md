VSCODE小技巧： Ctrl + D + D... 选中并编辑多个相同单词

1. background系列
   1.1 background-image
       url()

   1.1 使用两个background-image属性--使用逗号连接
   background-image: linear-gradient(
        to right bottom, 
        rgba(126, 213, 111, 0.8), 
        rgba(40, 180, 131, 0.8)), 
    url(../image/hero.jpg);
    上层是渐变色，下层是图片

   1.2 background-position: top | right | bottom | right;
       为背景图片设置初始位置。这个位置是相对于由 background-origin 定义的位置图层的。
       设为top则图片上缘紧贴盒子上缘，盒子大小变化时也一直保持上缘紧贴。除了keyword values，还可以设置percentage values, length values, multiple values等
   1.3 background-size: cover | contain;
       设置一个长度值，默认为宽，高度auto；设置两个长度值，为宽+高；给多个背景设置值，用逗号分隔。

2. clip-path: polygon(x y, x y, x y, x y);
    裁剪

3. h1是页面上最重要的标题，对搜索引擎很重要。可以通过span分隔的方式，设置语义连贯但样式不同的文字

4. 动画的两种创建方式
①@keyframes关键帧动画
创建动画：
  为了浏览器性能，最好只给动画添加两个属性。

使用动画：
  必填属性animation-name动画名和animation-duration动画持续时间。
  其他属性：animation-delay: 3s;\animation-interation-count: infinite;\animation-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1);
  backface-visibility: hidden;可以消除动画结束时的小闪动

  animation-fill-mode: backwards; 使动画元素在动画开始之前自动处于100%的状态

②transition属性
  transition-property，transition-duration，transition-timing-function 和 transition-delay的简写形式。
  为一个元素在不同状态之间切换的时候定义不同的过渡效果，为多属性指定时用冒号分割。
  需要设置在原始状态下。

5. pseudo-classes are a special state of a selector伪类是选择器的一种特殊状态
  ::after伪元素要显示在页面上时，必须为其添加content和display属性。
  伪元素可以看做原元素的子元素。

6. .btn:hover::after指的是当btn hover时才会出现这个伪元素，和.btn::after:hover不一样

7. 淡入淡出效果，可以通过设置opacity实现

布局技巧：
1. img是行内元素，常在其外包裹一个div，便于布局;alt属性利于SEO（Search Engine Optimization搜索引擎优化)，也用于图片无法加载的情况

2. 使用absolute(top/left)定位和transform: translate()配合，使元素垂直水平居中

3. text-align: center; 可以使盒子（block,table-cell）的内容水平居中