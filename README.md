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


