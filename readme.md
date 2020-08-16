## VideoCalling

p2p局域网音视频通话的demo，只需要对方的ip，端口和绑定本地端口，即可实现直连的视频聊天！

### 更新日志
#### 2017-12-13日项目成立
主要借鉴于开源项目  https://github.com/liuqm/Android-VideoChat-master 学习的相关知识，非常感谢大神的贡献，所以本人从开源社区学习，也回馈开源社区

#### 2018-1-31
发布初版，主要使用java nio传输视频数据，加入音频

#### 2018-11-15
使用了netty传输音视频数据，使用了speex降噪,使用了x264软编，mediacodec硬遍，ffmpeg软解，mediacodec硬解码的来处理yuv数据，之间传输的数据类型是h264
#### 2019-08-26
优化代码结构，添加opengl的代码，里面编解码请在代码层次自己选择使用
- FFmpegDecoder 是ffmpeg软解
- HardwareDecoder是 硬解（直接绑定serfaceview渲染）
- YUVHardwareDecoder是 硬解出yuv数据交给其他第三方渲染

- X264Encoder x264软编
- HardwareEncoder 硬编码

### 



### 后续发展
项目未来的方向是解决以下几个问题：第一，视频传输丢包的问题，第二，服务器打洞部署到外网上，第三，h265的编解码研究，第四，消回音的处理！，目前作者正在学习当中，也希望大家有
相关的资料或者方向能指点一下，感激不尽，最后祝各位程序员家庭和睦，幸福美满！

