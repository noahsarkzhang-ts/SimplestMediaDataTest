# SimplestMediaDataTest
**改动的地方：**

- 将开发环境由 VC++ 改为 Clion 环境。

## 代码说明

本项目包含如下几种视音频测试示例：

- (1)像素数据处理程序。包含RGB和YUV像素格式处理的函数。
- (2)音频采样数据处理程序。包含PCM音频采样格式处理的函数。
- (3)H.264码流分析程序。可以分离并解析NALU。
- (4)AAC码流分析程序。可以分离并解析ADTS帧。
- (5)FLV封装格式分析程序。可以将FLV中的MP3音频码流分离出来。
- (6)UDP-RTP协议分析程序。可以将分析UDP/RTP/MPEG-TS数据包。

This project contains following samples to handling multimedia data:

- (1) Video pixel data handling program. It contains several examples to handle RGB and YUV data.
- (2) Audio sample data handling program. It contains several examples to handle PCM data.
- (3) H.264 stream analysis program. It can parse H.264 bitstream and analysis NALU of stream.
- (4) AAC stream analysis program. It can parse AAC bitstream and analysis ADTS frame of stream.
- (5) FLV format analysis program. It can analysis FLV file and extract MP3 audio stream.
- (6) UDP-RTP protocol analysis program. It can analysis UDP/RTP/MPEG-TS Packet.

## 雷霄骅大佬源文地址

1. [视音频数据处理入门：RGB、YUV像素数据处理](https://blog.csdn.net/leixiaohua1020/article/details/50534150)
2. [视音频数据处理入门：PCM音频采样数据处理](https://blog.csdn.net/leixiaohua1020/article/details/50534316)
3. [视音频数据处理入门：H.264视频码流解析](https://blog.csdn.net/leixiaohua1020/article/details/50534369)
4. [视音频数据处理入门：AAC音频码流解析](https://blog.csdn.net/leixiaohua1020/article/details/50535042)
5. [视音频数据处理入门：FLV封装格式解析](https://blog.csdn.net/leixiaohua1020/article/details/50535082)
6. [视音频数据处理入门：UDP-RTP协议解析](https://blog.csdn.net/leixiaohua1020/article/details/50535230)