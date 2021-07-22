# # 百分百猜拳王简介



## 背景

​	该项目为2021年RTT嵌入式AI暑假学校的为期三天的开发马拉松作业

## 目标功能

​	通过神经网络的方法实现对剪刀、石头、布的实现，并将神经网络模型部署到嵌入式设备上。嵌入式设备通过摄像头实时识别屏幕中的人手的姿态（剪刀、石头、布），最后根据游戏规则设备显示能取胜的手势。

## 硬件

[AT-PI](https://art-pi.gitee.io/website/)

![AR_AK](E:\DIY\NICT_AI\Embedded-AI\picture\AR_AK.png)

   

[AT-PI多媒体扩展板]()

![image-20210722180515521](E:\DIY\NICT_AI\Embedded-AI\picture\image-20210722180515521.png)

## 软件

* RT_PI编程环境：RT-Thread Studio
* AI转换工具：AT-AK

## 目录结构

--BSP：AT-PI代码工程

--data:数据集（[获取网站](https://laurencemoroney.com/datasets.html)）

---model :模型文件

--picture：图片

--pythoh_code：神经网络模型

## 实现效果

网络为量化之前的准确率为88.49%。模型经过量化后部署到单片机上，基本上能实现识别石头、剪刀、布的功能，但是准确度有所下降。

## 优化方向

* 数据集为外国人搜集，其手势布适合国人习惯，可以自己制作数据集。
* 网络模型过于简单，训练次数过于少。在增加数据集的基础上可以加深网络结构

