# JumpBubble

酷炫实用的态度气泡，通过canvas实现

### [点我预览效果吧](https://wanghairong-i.github.io/JumpBubble/)

## 介绍

-   该插件无任何依赖，纯原生js写成
-   API丰富，使用简单，可设置气泡的大小、气泡浮动效果、位置等多种自定义效果
-   创建态度气泡时，你只需关心数据，即用于创建气泡的src路径或cnd地址，无需手动创建img标签，JumpBubble会帮你生成为指定大小表情
-   冒泡的生命周期完善，初始化容器时，开始冒泡前、冒泡结束时等阶段都可设置回调函数
-   兼容IE9+
-   webpack + es6 跑项目

## 项目怎么跑起来？  HOW TO RUN

```javascript

//安装
npm install  

//启动
npm start

//产出
npm run build

```

## 怎么使用插件？ HOW TO USE

```javascript

//初始化
const bubble = new JumpBubble(canvasNode);

//调用实例的create方法，每次传入想要冒泡的图像的src即可，无需手动创建多余的img标签
//src可以是cdn地址，也可以是相对路径（相对路径是相对html文件）或绝对路径
bubble.create(imgsrcStr);

```

### 实例

#### html 

```html

<!-- 注意指定宽高 -->
<canvas id="cavs" width="150" height="400" >您的浏览器不支持canvas标签~</canvas>

```

#### JS

```javascript

const bubble = new JumpBubble(document.getElementById('cavs'));

bubble.create('http://p8.qhimg.com/t01053ab4d4d6510abd.png'); //此处src为cnd地址

```

### 好了，完成了，快去看看效果吧
