# 1. B/S和C/S
1. 浏览器/服务器 教务系统
2. 客户端/服务器 
# 2. 优缺点
1. 开发/维护成本		B/S相对低 
2. 运算负载			C/S可以使用客户端分担压力
3. 安全性			专人专用客户端（银行）  C/S
# 3.【面试】网页的呈现过程
	URL验证 --> DNS解析  --> TCP三次握手（建立连接）  --> 处理请求 --> 渲染页面 --> 断开连接
# 4.【重点】URL格式
	协议://主机地址（域名或IP地址）:端口号/资源路径?参数名1=参数值1&参数名2=参数值2&……#书签（信息片段）
	eg: https://www.baidu.com:443
## 1. 协议
1. http 超文本传输协议
2. https 在链路层上套接字加密的超文本传输协议（安全的http）
3. ftp 文件传输协议 
## 2. ip地址：本机ip地址 127.0.0.1 localhost
## 3. 端口号
1. http默认端口 80
2. MySQL端口 3306
3. Tomcat 服务器容器 8080
## 4. 资源路径
1. 首页 缺省 index.html  index.php index.jsp
2. 参数的传递
3. 书签
## 5. URL、URI、URN
1. URL 统一资源定位器
2. URI 统一资源标识（ID）
3. URN 统一资源命名
4. 注意
  1. URI范围最大
  2. URL不支持中文
# 5. MIME 一级类型/二级类型
1. text 文本   text/html
2. image 图像  image/jpg image/png
3. audio 音频
4. video 视频
5. application 应用 
6. message 报文信息
7. multipart 多部分媒体（文件上传）eg. 用户注册

	