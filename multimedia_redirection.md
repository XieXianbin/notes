## 多媒体重定向


桌面云视频播放有两种方式：
1）服务端渲染，顾名思义，是用虚拟机的CPU进行编解码、渲染后，发送到瘦终端进行显示，传的是图像，这是对虚拟机的CPU消耗就大；
2）多媒体重定向，也可以称 客户端渲染，视频文件是经过 分片、打包、通过Spice协议传输到瘦终端，利用瘦终端上的播放器程序进行播放的，因此虚拟机的CPU消耗基本忽略不计，可以提高整个虚拟机的视频并发密度；