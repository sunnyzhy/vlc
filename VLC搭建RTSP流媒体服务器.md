### 简介
VLC官网：<font color=#0099ff>http://www.videolan.org/vlc/</font>

VLC不仅可以作为播放器，还可以作为流媒体服务器使用。

### 用VLC搭建基于RTSP的流媒体服务器
#### 一、搭建流媒体服务器
1.打开VLC，选择"<font color=#0099ff>媒体 -> 流</font>"

![](/images/1.png)

2.选择"捕获设备 -> 适配设备名称"，点击"串流"

![](/images/2.png)

3.点击"下一个"

![](/images/3.png)

4.选择"<font color=#0099ff>RTSP</font>"，点"添加"

![](/images/4.png)

5.输入端口号和路径，点"下一个"

![](/images/5.png)

6.选择"<font color=#0099ff>Video - H.264 + MP3 (MP4)</font>"，点"下一个"

![](/images/6.png)

7.生成串流输出字符串，点击"流"

![](/images/7.png)

8.如果VLC的标题栏显示"<font color=#0099ff>流</font>"，就说明流服务器已经搭建成功

![](/images/8.png)

#### 二、客户端播放视频

1.打开VLC作为视频播放器的客户端，选择"<font color=#0099ff>媒体 -> 打开网络串流</font>"

![](/images/9.png)

2.选择"网络"，输入网络URL"<font color=#0099ff>rtsp://127.0.0.1:8554/stream</font>"，其中，<font color=#0099ff>8554</font>和<font color=#0099ff>stream</font>是在搭建RTSP流媒体服务器时填写的<font color=#0099ff>端口号</font>和<font color=#0099ff>路径</font>，点击"播放"

![](/images/10.png)

3.预览视频

![](/images/11.png)