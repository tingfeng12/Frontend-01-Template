# 每周总结可以写在这里
对浏览器的实现者来说，他们做的事情，就是把一个 URL 变成一个屏幕上显示的网页。这个过程是这样的：浏览器首先使用 HTTP 协议或者 HTTPS 协议，向服务端请求页面；把请求回来的 HTML 代码经过解析，构建成 DOM 树；计算 DOM 树上的 CSS 属性；最后根据 CSS 属性对元素逐个进行渲染，得到内存中的位图；一个可选的步骤是对位图进行合成，这会极大地增加后续绘制的速度；合成之后，再绘制到界面上。

HTTP 协议
HTTP 协议格式
HTTP Method（方法）
HTTP Status code（状态码）和 Status text（状态文本）
HTTP Head (HTTP 头)
HTTP Request Body
HTTPS
HTTP 2