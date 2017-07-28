### 简介
VLC官网：**http://www.videolan.org/vlc/**

VLC不仅可以作为播放器，还可以作为流媒体服务器使用。

### 用VLC搭建基于HTTP的流媒体服务器
####

![](/images/20.png)

#### 一、搭建流媒体服务器
1.打开VLC，选择**"媒体 -> 流"**

![](/images/1.png)

2.选择"网络"，输入**RTSP流服务器的URL**，点击"串流"

![](/images/12.png)

3.点击"下一个"

![](/images/13.png)

4.选择**"HTTP"**，点"添加"

![](/images/14.png)

5.输入端口号和路径，点"下一个"

![](/images/15.png)

6.选择**"Video - Theora + Vorbis (OGG)"**，点"下一个"

![](/images/16.png)

7.生成串流输出字符串，点击"流"

![](/images/17.png)

8.如果VLC的标题栏显示**"流"**，就说明流服务器已经搭建成功

![](/images/18.png)

#### 二、浏览器播放视频
1.在html5里嵌入video标签，source属性为**"http://127.0.0.1:8080/stream"**

	<!DOCTYPE html>
	<html>
		<head>
			<meta charset="UTF-8">
			<title>Media</title>
		</head>
		<body>
			<video controls autoplay width="600" height="250">  
  				<source src="http://127.0.0.1:8080/stream" type="video/ogg">
  				Your browser does not support the video tag.
			</video>
		</body>
	</html>

2.在浏览器的地址栏里输入**"http://127.0.0.1/media.html"**，预览视频

![](/images/19.png)