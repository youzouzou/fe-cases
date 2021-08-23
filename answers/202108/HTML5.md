### （1）语义化标签
<table style="width: 552px" border="0">
  <tbody>
    <tr>
      <td style="text-align: center">
        <span style="font-size: 15px">&nbsp;标签</span></td>
      <td style="text-align: center">
        <span style="font-size: 15px">&nbsp;描述</span></td>
    </tr>
    <tr>
      <td style="text-align: center">&nbsp;&lt;hrader&gt;&lt;/header&gt;</td>
      <td style="text-align: center">&nbsp;定义了文档的头部区域</td></tr>
    <tr>
      <td style="text-align: center">&nbsp;&lt;footer&gt;&lt;/footer&gt;</td>
      <td style="text-align: center">&nbsp;定义了文档的尾部区域</td></tr>
    <tr>
      <td style="text-align: center">&lt;nav&gt;&lt;/nav&gt;</td>
      <td style="text-align: center">定义文档的导航</td></tr>
    <tr>
      <td style="text-align: center">&nbsp;&lt;section&gt;&lt;/section&gt;</td>
      <td style="text-align: center">&nbsp;定义文档中的节（section、区段）</td></tr>
    <tr>
      <td style="text-align: center">&nbsp;&lt;article&gt;&lt;/article&gt;</td>
      <td style="text-align: center">&nbsp;定义页面独立的内容区域</td></tr>
    <tr>
      <td style="text-align: center">&lt;aside&gt;&lt;/aside&gt;</td>
      <td style="text-align: center">定义页面的侧边栏内容</td></tr>
    <tr>
      <td style="text-align: center">&lt;detailes&gt;&lt;/detailes&gt;</td>
      <td style="text-align: center">用于描述文档或文档某个部分的细节</td></tr>
    <tr>
      <td style="text-align: center">&lt;summary&gt;&lt;/summary&gt;</td>
      <td style="text-align: center">标签包含 details 元素的标题</td></tr>
    <tr>
      <td style="text-align: center">&lt;dialog&gt;&lt;/dialog&gt;</td>
      <td style="text-align: center">定义对话框，比如提示框</td></tr>
  </tbody>
</table>### （2）增强型表单
<table style="width: 557px" border="0">
  <tbody>
    <tr>
      <td>
        <p style="text-align: center">输入类型</p></td>
      <td style="text-align: center">描述</td></tr>
    <tr>
      <td>
        <p style="text-align: center">color</p></td>
      <td style="text-align: center">主要用于选取颜色</td></tr>
    <tr>
      <td>
        <p style="text-align: center">date</p></td>
      <td style="text-align: center">从一个日期选择器选择一个日期</td></tr>
    <tr>
      <td>
        <p style="text-align: center">datetime</p></td>
      <td style="text-align: center">选择一个日期（UTC 时间）</td></tr>
    <tr>
      <td>
        <p style="text-align: center">datetime-local</p></td>
      <td style="text-align: center">选择一个日期和时间 (无时区)</td></tr>
    <tr>
      <td>
        <p style="text-align: center">email</p></td>
      <td style="text-align: center">包含 e-mail 地址的输入域</td></tr>
    <tr>
      <td>
        <p style="text-align: center">month</p></td>
      <td style="text-align: center">选择一个月份</td></tr>
    <tr>
      <td>
        <p style="text-align: center">number</p></td>
      <td style="text-align: center">数值的输入域</td></tr>
    <tr>
      <td>
        <p style="text-align: center">range</p></td>
      <td style="text-align: center">一定范围内数字值的输入域</td></tr>
    <tr>
      <td>
        <p style="text-align: center">search</p></td>
      <td style="text-align: center">用于搜索域</td></tr>
    <tr>
      <td>
        <p style="text-align: center">tel</p></td>
      <td style="text-align: center">定义输入电话号码字段</td></tr>
    <tr>
      <td>
        <p style="text-align: center">time</p></td>
      <td style="text-align: center">选择一个时间</td></tr>
    <tr>
      <td>
        <p style="text-align: center">url</p></td>
      <td style="text-align: center">&nbsp;URL 地址的输入域</td></tr>
    <tr>
      <td>
        <p style="text-align: center">week</p></td>
      <td style="text-align: center">选择周和年</td></tr>
  </tbody>
</table>

HTML5 新增的表单属性
- placehoder 属性，简短的提示在用户输入值前会显示在输入域上。即我们常见的输入框默认提示，在用户输入后消失。
- required 属性，是一个 boolean 属性。要求填写的输入域不能为空
- pattern 属性，描述了一个正则表达式用于验证 `<input>` 元素的值。
- min 和 max 属性，设置元素最小值与最大值。
- step 属性，为输入域规定合法的数字间隔。
- height 和 width 属性，用于 image 类型的 `<input>` 标签的图像高度和宽度。
- autofocus 属性，是一个 boolean 属性。规定在页面加载时，域自动地获得焦点。
- multiple 属性 ，是一个 boolean 属性。规定`<input>` 元素中可选择多个值。　　　

### （3）视频和音频
```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
您的浏览器不支持Video标签。
</video>

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
您的浏览器不支持 audio 元素。
</audio>
```

### （4）Canvas
```html
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>

<script>
　　var c=document.getElementById("myCanvas");
　　var ctx=c.getContext("2d");
　　ctx.fillStyle="#FF0000";
　　ctx.fillRect(0,0,150,75);
</script>
```

### （5）SVG绘图
可伸缩的矢量图形

### （6）地理定位
```js
var x = document.getElementById("demo");
function getLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(showPosition);
    }
    else {
        x.innerHTML = "该浏览器不支持获取地理位置。";
    }
}

function showPosition(position) {
    x.innerHTML = "纬度: " + position.coords.latitude +
        "<br>经度: " + position.coords.longitude;
}
```

### （7）拖放API
拖放的源对象(可能发生移动的)可以触发的事件——3个：
- dragstart：拖动开始
- drag：拖动中
- dragend：拖动结束

整个拖动过程的组成： dragstart*1 + drag*n + dragend*1


拖放的目标对象(不会发生移动)可以触发的事件——4个：
- dragenter：拖动着进入
- dragover：拖动着悬停
- dragleave：拖动着离开
- drop：释放

整个拖动过程的组成1： dragenter*1 + dragover*n + dragleave*1

整个拖动过程的组成2： dragenter*1 + dragover*n + drop*1

### （8）Web Worker

### （9）Web Storage
localStorage和sessionStorage

### （10）WebSocket
WebSocket使得服务器可以主动向客户端推送信息，客户端也可以主动向服务器发送信息，是真正的双向平等对话，属于服务器推送技术的一种。

（1）建立在 TCP 协议之上，服务器端的实现比较容易。

（2）与 HTTP 协议有着良好的兼容性。默认端口也是80和443，并且握手阶段采用 HTTP 协议，因此握手时不容易屏蔽，能通过各种 HTTP 代理服务器。

（3）数据格式比较轻量，性能开销小，通信高效。

（4）可以发送文本，也可以发送二进制数据。

（5）没有同源限制，客户端可以与任意服务器通信。

（6）协议标识符是ws（如果加密，则为wss），服务器网址就是 URL。

```js
var ws = new WebSocket("wss://echo.websocket.org");

ws.onopen = function(evt) { 
  console.log("Connection open ..."); 
  ws.send("Hello WebSockets!");
};

ws.onmessage = function(evt) {
  console.log( "Received Message: " + evt.data);
  ws.close();
};

ws.onclose = function(evt) {
  console.log("Connection closed.");
};      
```

---

参考：
1. https://www.cnblogs.com/vicky1018/p/7705223.html
2. https://www.ruanyifeng.com/blog/2017/05/websocket.html