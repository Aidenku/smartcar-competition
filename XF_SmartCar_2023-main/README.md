#  XJTLU GMaster Club XF Smart Car Team

## 简介
本项目代码面向2023全国智能汽车大赛 讯飞机器人 智慧农业赛道。<br>
## 介绍
## 👨‍💻 我的职责

我在本项目中主要负责以下核心模块的设计与代码实现：
- **自主导航与避障算法**
- **路径规划策略与调试**
- **激光雷达 SLAM 系统集成**
- **语音播报逻辑编写与调试**
  
## 环境配置
### 视觉环境配置
+ 配置[Jetson Inference](https://github.com/dusty-nv/jetson-inference)
    + 请按照github官方文档，使用源码编译的方式进行配置
    + 不要安装任何的模型权重文件
    + 不要安装任何的demo
    + 不要安装pytorch
+ 配置权重文件
  +  将权重文件```car.onnx```和标记文件```label.txt```放入```classify_net```文件夹中的car.onnx文件放入```src```文件夹中的```ar_code_server.cpp```中这行代码的位置
      ```
     imageNet *net = imageNet::Create(NULL, "your car.onnx", NULL, "your label.txt", "input", "output");
      ```
  + 请使用绝对路径
## 参赛人员
| 张昱轩 | 数据科学与大数据技术 | Yuxuan.Zhang2104@student.xjtlu.edu.cn 
| 顾羚旦 | 机器人工程 | Lingdan.Gu21@student.xjtlu.edu.cn     
| 任晋昊 | 数据科学与大数据技术 | Jinhao.Ren21@student.xjtlu.edu.cn     
| 梁森韦 | 数据科学与大数据技术 | Jinhao.Ren19@student.xjtlu.edu.cn     
| 王奕方 | 数据科学与大数据技术 | Yifang.Wang21@student.xjtlu.edu.cn    
