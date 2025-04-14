# 🚗 SmartCar Competition 2023

## 🏫 XJTLU GMaster Club - XF Smart Car Team

This repository contains the full source code and documentation for our participation in the **2023 National SmartCar Competition**, specifically in the **iFLYTEK Robotics – Smart Agriculture Track**.

---

## 📌 Project Overview

This project features an intelligent autonomous vehicle designed for smart agricultural tasks, integrating the following core functionalities:

- 🔍 Autonomous navigation based on real-time sensor input
- 🧠 Path planning for dynamic route adjustments
- 📡 LiDAR-based SLAM (Simultaneous Localization and Mapping)
- 🔊 Voice broadcasting system for real-time feedback

---

## 👨‍💻 My Responsibilities

As a core team member, I was responsible for the following modules:

- 🚗 Autonomous navigation and obstacle avoidance algorithms
- 🧭 Path planning strategy design and tuning
- 🗺️ SLAM system integration using LiDAR
- 📢 Voice broadcasting logic implementation and debugging

---

## ⚙️ Environment Setup

### ▶️ Visual Inference Module (Jetson Platform)

We use [Jetson Inference](https://github.com/dusty-nv/jetson-inference) for vehicle and object recognition.

#### Setup Instructions

1. Clone and **build Jetson Inference from source** using the official GitHub guide
2. **Do not** install:
   - Pre-trained model weights
   - Demo applications
   - PyTorch (install separately if needed)
3. Download model weights:
   - Place `car.onnx` and `label.txt` inside the `classify_net` folder
   - Modify the following line in `src/ar_code_server.cpp` with **absolute paths**:

```cpp
imageNet *net = imageNet::Create(NULL, "your_absolute_path/car.onnx", NULL, "your_absolute_path/label.txt", "input", "output");

## 👥 Team Members

We are a multidisciplinary team of undergraduate students from Xi’an Jiaotong-Liverpool University (XJTLU), working together under the GMaster Club to participate in the 2023 XF SmartCar Competition – Smart Agriculture Track.

| Name            | Major                                | Email                                   | Responsibility Highlights                  |
|------------------|----------------------------------------|------------------------------------------|---------------------------------------------|
| **Lingdan Gu**     | Intelligent Robotics Engineering        | Lingdan.Gu21@student.xjtlu.edu.cn        | SLAM, navigation, path planning, voice system |
| **Yuxuan Zhang**   | Data Science and Big Data Technology    | Yuxuan.Zhang2104@student.xjtlu.edu.cn    | Machine learning, Computer vision     |
| **Jinhao Ren**     | Data Science and Big Data Technology    | Jinhao.Ren21@student.xjtlu.edu.cn        | Data processing, system testing             |
| **Senwei Liang**   | Data Science and Big Data Technology    | Jinhao.Ren19@student.xjtlu.edu.cn        | voice system, Code framework construction    |
| **Yifang Wang**    | Data Science and Big Data Technology    | Yifang.Wang21@student.xjtlu.edu.cn       | Adjust parameters, path planning|

