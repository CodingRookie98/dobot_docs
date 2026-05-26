# Dobot edu API (Python SDK) 开发接口文档 (v2.2.2)

> [!NOTE]
> **本 Python SDK 接口文档已完成全量完善与模块化重构**。
>
> 我们已将军端/官方在线文档库（DobotLab Coding Manual）中关于 **3. Python编程指令** 的 183 个页面全部同步并清洗，按模块分流整合到以下 9 个子文档中。本主文档作为 Python 接口开发的**全局导航首页**。

---

## 1. 模块化文档全局索引

请点击下方链接直达各硬件与服务模块的详细 API 定义：

### 🤖 机器人与外设控制接口
*   [**3.1 Dobot Magician Lite 机械臂控制**](01_Dobot_Magician_Lite.md) —— 点到点运动（PTP）、吸嘴/夹爪状态控制、回零、实时坐标与丢步检测。
*   [**3.4 Dobot Magician Go 基础小车控制**](04_Dobot_Magician_Go.md) —— 全向移动速度、旋转、巡线控制（PID）、超声波/里程计/IMU 传感器数据及灯效蜂鸣器。
*   [**3.5 Dobot Magician Go Beta 复合控制**](05_Dobot_Magician_Go_Beta.md) —— 自动出入库、物品抓取、机械臂/小车摄像头识别模型配置及坐标转换。
*   [**3.6 Dobot Magician 接口指令**](06_Dobot_Magician.md) —— 第二代经典 Magician 机械臂的运动与 IO 信号接口定义。
*   [**3.7 Dobot Magic Box 与基础外设**](07_Dobot_Magic_Box.md) —— 本地麦克风录音、摄像头拍照获取等基础外设工具（`util`）和控制。

---

### 🧩 传感器与 AI 云服务接口
*   [**3.2 AI 传感器套件接口**](02_AI_传感器套件接口.md) —— OLED屏幕显示、LED灯光控制、声音播放及旋钮/光线/温湿度/手势/人体传感器读数。
*   [**3.3 AI 模块服务指令**](03_AI_模块.md) —— 语音识别（ASR）、在线合成（TTS）、NLP主题分析、机器翻译及人脸检测比对。
*   [**3.8 图像识别与分类**](08_图像识别.md) —— 云端图像特征提取、分类器切图及目标检测算法相关。

---

### 💡 官方应用示例
*   [**3.9 Python程序集成示例**](09_Python程序示例.md) —— 官方集成的 Python 二次开发经典流程伪代码及避坑指南。
