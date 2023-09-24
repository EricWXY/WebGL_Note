# WebGL_Note
学习 WebGL 以及 threejs 的个人笔记


## canvas 和 webgl 的区别

### 1.1 `<canvas>` 画布

- `<canvas></canvas>` 是 HTML5 新增的一个 DOM 元素

用途： 展示 <b>二维</b> 和 <b>三维</b> 的图像

- 绘制：二维图形<b>可以使用 （Canvas API 或 WebGL API）</b>
        三维图形<b>使用 WebGL API</b>

### 1.2 Canvas API

- Canvas API 提供二维绘图的方式

- 图形的绘制主要通过 `CanvasRenderingContext2D` 接口完成

- `canvas.getContext('2d')`

### 1.3 WebGL API

- WebGL API 提供三维绘图的方式

- 图形的绘制主要通过 `WebGLRenderingContext` 接口完成

- `canvas.getContext('webgl')`

- `WebGL2RenderingContext` `canvas.getContext('webgl2')`

### 总结

Canvas和WebGL是两种用于在Web浏览器上进行图形渲染的技术，它们有一些区别和联系：

区别：

API：Canvas使用2D绘图API，而WebGL使用底层的3D图形API。
功能：Canvas适用于绘制2D图形，例如绘制图像、绘制形状和文字等。相比之下，WebGL提供了更强大的功能，可以进行高性能的3D图形渲染，包括复杂的光照、纹理映射和深度测试等。
学习曲线：Canvas的学习曲线相对较低，更容易上手。WebGL则需要对图形编程和着色器有一定的了解，学习曲线较陡。
兼容性：Canvas是HTML5的一部分，几乎所有现代浏览器都支持。WebGL则基于OpenGL ES标准，需要浏览器支持WebGL扩展才能运行。
联系：

共同点：Canvas和WebGL都是基于HTML5的技术，用于在Web浏览器中进行图形渲染。
嵌入：WebGL是Canvas的一种扩展，可以在Canvas元素中创建WebGL上下文，实现高性能的3D图形渲染。
交互：Canvas和WebGL都可以通过JavaScript代码进行交互，实现动态的图形渲染和用户交互。
总的来说，Canvas适用于简单的2D图形绘制，而WebGL则提供了更强大的3D图形渲染功能。选择使用哪种技术取决于需求和技术要求。如果只需要进行简单的2D绘制，那么使用Canvas就足够了；如果需要进行复杂的3D图形渲染，那么WebGL是更好的选择。


-------------------------------------------------------------------

## WebGL 简介

- 什么是 WebGL
- 为什么学习 WebGL
- WebGL 的优势
- 学习前置条件
- WebGL 程序结构
- WebGl 开源框架

### 2.1 什么是 WebGL

- WebGL 是一种`3D绘图协议`，衍生于 OpenGL ES2.0，可以结合HTML5 和 Javascript 在网页上绘制和渲染二/三维图形

### 2.2 为什么学习 WebGL

- 数据可视化
- 图形/游戏引擎
- 交互演示、图形渲染
- 地图
- VR
- 物品展示/室内设计
- 城市规划
- 想象力还很丰富...

### 2.3 WebGL 的优势

- 内嵌浏览器，不需要安装任何插件或环境即可运行
- 只需要一个文本编辑器和浏览器，就可以编写三维图形程序

### 2.4 前置条件

- 文本编辑器
- 浏览器
- HTML 和 JS 基础


### 2.5 程序结构

<img src="./imgs/WebGL 程序结构.png">


> GLSL ES (着色器程序) 是以`字符串`的形式存在 JS 中

### 2.6 WebGL 开源框架

- Three.js : JavaScript 3D WebGL 库
- Babylon.js : Web3D 图形引擎
- KickJS : Web 的开源图形和游戏引擎
- ClayGL : 构建可扩展的 Web3D 应用程序
- PlayCanvas : 网络游戏和3D图形引擎
- WebGLStudio.js 和 Litescene.js : 开源Web3D 图形编辑器和创建器
- Luma : Uber 的 3D WebGL 可视化库
- A-Frame : 用于构建 VR 的 Web 框架