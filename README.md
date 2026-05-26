# Dobot 机器人开发文档库

本仓库用于管理和维护 Dobot 工业机器人的各类开发手册与接口文档。目前已完成了以下四大接口文档的全量 Markdown 模块化接入、校对与优化：

1.  **Dobot TCP/IP 二次开发接口文档 (V4.6.0)**
2.  **Dobot edu API (Python SDK) 开发接口文档 (v2.2.2)**
3.  **DobotLink API 开发接口文档 (CHM 转换中文版)**
4.  **DobotLink API English Version Documentation (CHM 转换英文版)**

---

## 📂 目录结构说明

```text
├── pdf/                            # 官方原始 PDF 物理文档
│   └── Dobot_TCP_IP二次开发接口文档V4.6.0_2024.12.26_cn.pdf
├── CHM/                            # 官方原始 CHM 帮助文档
│   ├── DobotLinkHelp.CHM
│   └── DobotLinkHelp_EN.CHM
├── md/                             # Markdown 电子化版本
│   ├── Dobot_TCP_IP_v4.6.0/        # TCP/IP 模块化文档目录
│   │   ├── README.md               # TCP/IP 导航首页 (Index)
│   │   └── 01_前言与概述.md 等...
│   ├── Dobot_edu_api/              # Python SDK 模块化文档目录
│   │   ├── README.md               # Python SDK 导航首页 (Index)
│   │   └── 01_Dobot_Magician_Lite.md 等...
│   ├── DobotLinkHelp/              # DobotLink API 模块化文档目录 (中文版)
│   │   ├── README.md               # DobotLink 中文导航首页 (README)
│   │   └── index.md                # 全量 API 字母顺序索引页
│   └── DobotLinkHelp_EN/           # DobotLink API 模块化文档目录 (英文版)
│       ├── README.md               # DobotLink 英文导航首页 (README)
│       └── index.md                # 全量 API 字母顺序索引页
└── README.md                       # 本说明文件 (仓库全局导引)
```

---

## 🚀 核心文档直达

*   👉 [**Dobot TCP/IP 二次开发接口文档 (V4.6.0) 导航首页**](md/Dobot_TCP_IP_v4.6.0/README.md)
*   👉 [**Dobot edu API (Python SDK) 接口文档 (v2.2.2) 导航首页**](md/Dobot_edu_api/README.md)
*   👉 [**DobotLink API 接口文档 (CHM 转换中文版) 导航首页**](md/DobotLinkHelp/README.md)
*   👉 [**DobotLink API English Version Documentation Navigation Index**](md/DobotLinkHelp_EN/README.md)

---

## 📋 模块化 Markdown 文档状态与校验表

### 1. Dobot TCP/IP 接口文档 (V4.6.0)

以下是 `md/Dobot_TCP_IP_v4.6.0/` 子目录下所有子文档的状态：

| 子文档名称 | 对应 PDF 章节 | 内容完整度 | 校验状态 | 详细备注 / 统计数据 |
| :--- | :--- | :---: | :---: | :--- |
| [**01_前言与概述.md**](md/Dobot_TCP_IP_v4.6.0/01_前言与概述.md) | 前言、1 概述 | **全量完整** | ✅ 已校验 | 包含开发目的、读者对象及修订记录 |
| [**02_通讯架构与协议说明.md**](md/Dobot_TCP_IP_v4.6.0/02_通讯架构与协议说明.md) | 1 概述 (端口与格式) | **全量完整** | ✅ 已校验 | 包含交互端口列表与消息命令应答格式说明 |
| [**03_1_机器人系统控制.md**](md/Dobot_TCP_IP_v4.6.0/03_1_机器人系统控制.md) | 2.1 控制相关指令 | **全量完整** | ✅ 已校验 | 包含 `PowerOn` 等 **13 个** 接口详情 |
| [**03_2_设置相关指令.md**](md/Dobot_TCP_IP_v4.6.0/03_2_设置相关指令.md) | 2.2 设置相关指令 | **全量完整** | ✅ 已校验 | 包含 `SpeedFactor` 等 **21 个** 接口详情 |
| [**03_3_信息查询与运动学计算.md**](md/Dobot_TCP_IP_v4.6.0/03_3_信息查询与运动学计算.md) | 2.3 计算和获取指令 | **全量完整** | ✅ 已校验 | 包含 `GetPose` 等 **8 个** 接口详情 |
| [**03_4_IO与外设控制.md**](md/Dobot_TCP_IP_v4.6.0/03_4_IO与外设控制.md) | 2.4 IO相关指令 | **全量完整** | ✅ 已校验 | 包含 `DOInstant`、`DOGroup` 等 **19 个** 接口详情 |
| [**03_5_Modbus与总线寄存器.md**](md/Dobot_TCP_IP_v4.6.0/03_5_Modbus与总线寄存器.md) | 2.5 和 2.6 相关指令 | **全量完整** | ✅ 已校验 | 包含 Modbus 及总线控制共 **18 个** 接口详情 |
| [**03_6_运动控制指令.md**](md/Dobot_TCP_IP_v4.6.0/03_6_运动控制指令.md) | 2.7 运动相关指令 | **全量完整** | ✅ 已校验 | 包含 `MovJ`、`ServoJ/P` 等 **21 个** 轨迹指令详情 |
| [**03_7_高级功能.md**](md/Dobot_TCP_IP_v4.6.0/03_7_高级功能.md) | 2.8, 2.9, 2.10 指令 | **全量完整** | ✅ 已校验 | 包含力控设置、焊接恢复及日志共 **21 个** 接口详情 |
| [**04_实时反馈接口详解.md**](md/Dobot_TCP_IP_v4.6.0/04_实时反馈接口详解.md) | 3 实时反馈信息 | **全量完整** | ✅ 已校验 | 完整映射 1440 字节包中的 **53 个** 反馈字段 |
| [**05_错误处理与故障排查.md**](md/Dobot_TCP_IP_v4.6.0/05_错误处理与故障排查.md) | 4 通用错误码 | **全量完整** | ✅ 已校验 | 整理了包含 V4.6.0 新增 `-8` 错误码的 **15 个** 返回值 |
| [**06_各状态下指令执行权限.md**](md/Dobot_TCP_IP_v4.6.0/06_各状态下指令执行权限.md) | 5 各状态下执行权限 | **全量完整** | ✅ 已校验 | 不同使能状态下的在线指令下发矩阵说明 |
| [**07_常见问题与示例.md**](md/Dobot_TCP_IP_v4.6.0/07_常见问题与示例.md) | 附录 (示例与避坑) | **概要提取** | ✅ 已校验 | 包含常见开发流程伪代码和参数错误避坑指南 |
| [**08_全速开发支持.md**](md/Dobot_TCP_IP_v4.6.0/08_全速开发支持.md) | 附录 (全速开发支持) | **概要提取** | ✅ 已校验 | 多线程开发与并发控制的安全建议 |

---

### 2. Dobot edu API (Python SDK) 接口文档 (v2.2.2)

以下是 `md/Dobot_edu_api/` 子目录下所有子文档与官方在线 Coding Manual 的对应关系及状态：

| 子文档名称 | 对应在线章节 | 内容完整度 | 校验状态 | 详细备注 / 统计数据 |
| :--- | :--- | :---: | :---: | :--- |
| [**01_Dobot_Magician_Lite.md**](md/Dobot_edu_api/01_Dobot_Magician_Lite.md) | 3.1 Magician Lite 机械臂 | **全量完整** | ✅ 已校验 | 包含 `m_lite` 的点到位运动、吸盘夹爪及回零共 **17 个** 主题 |
| [**02_AI_传感器套件接口.md**](md/Dobot_edu_api/02_AI_传感器套件接口.md) | 3.2 AI 传感器套件接口 | **全量完整** | ✅ 已校验 | 包含 OLED 显示、LED、声音及 14 个传感器共 **32 个** 接口 |
| [**03_AI_模块.md**](md/Dobot_edu_api/03_AI_模块.md) | 3.3 AI 模块 | **全量完整** | ✅ 已校验 | 包含人脸比对、OCR、ASR 语音技术和翻译共 **24 个** 接口 |
| [**04_Dobot_Magician_Go.md**](md/Dobot_edu_api/04_Dobot_Magician_Go.md) | 3.4 Dobot Magician Go | **全量完整** | ✅ 已校验 | 包含里程计、全向移动、巡线控制与蜂鸣器共 **24 个** 接口 |
| [**05_Dobot_Magician_Go_Beta.md**](md/Dobot_edu_api/05_Dobot_Magician_Go_Beta.md) | 3.5 Magician Go Beta | **全量完整** | ✅ 已校验 | 包含出入库、地板/车上物品抓取与坐标转化共 **18 个** 接口 |
| [**06_Dobot_Magician.md**](md/Dobot_edu_api/06_Dobot_Magician.md) | 3.6 Dobot Magician | **全量完整** | ✅ 已校验 | 包含第二代经典机械臂的滑轨点到位、吸盘与IO共 **29 个** 接口 |
| [**07_Dobot_Magic_Box.md**](md/Dobot_edu_api/07_Dobot_Magic_Box.md) | 3.7 Dobot Magic Box | **全量完整** | ✅ 已校验 | 包含滑轨运动、步进/传送带电机、蓝牙与外设共 **27 个** 接口 |
| [**08_图像识别.md**](md/Dobot_edu_api/08_图像识别.md) | 3.8 图像识别 | **全量完整** | ✅ 已校验 | 包含图片分割、颜色分类、背景校准与识别共 **9 个** 接口 |
| [**09_Python程序示例.md**](md/Dobot_edu_api/09_Python程序示例.md) | 3.9 Python程序示例 | **概要提取** | ✅ 已校验 | 包含官方经典代码示例与附录说明共 **3 个** 主题 |

---

### 3. DobotLink API 接口文档 (CHM 转换版)

以下是 `md/DobotLinkHelp/` 子目录下所有子目录及核心文件的状态：

| 子目录/文件名称 | 对应功能模块 | 内容完整度 | 校验状态 | 详细备注 / 统计数据 |
| :--- | :--- | :---: | :---: | :--- |
| [**1 前言**](md/DobotLinkHelp/1%20前言) | 前言与开发协议 | **全量完整** | ✅ 已校验 | 包含接口协议说明等入门前置知识 |
| [**2 DobotLink API**](md/DobotLinkHelp/2%20DobotLink%20API) | DobotLink 核心 API | **全量完整** | ✅ 已校验 | 包含 `CleanLogs`、`CloseDobotLink` 等 **12 个** 核心控制 API |
| [**3 Magician API**](md/DobotLinkHelp/3%20Magician%20API) | Magician 机械臂 | **全量完整** | ✅ 已校验 | 包含 PTP、JOG、IO 及传送带等 **44 个** API |
| [**4 MagicianLite API**](md/DobotLinkHelp/4%20MagicianLite%20API) | Magician Lite 机械臂 | **全量完整** | ✅ 已校验 | 包含点到位、滑轨、传送带、吸盘及通用 IO 共 **24 个** API |
| [**5 MagicBox API**](md/DobotLinkHelp/5%20MagicBox%20API) | Magic Box 控制箱 | **全量完整** | ✅ 已校验 | 包含电机参数、滑轨、手持示教及多传感器共 **30 个** API |
| [**6 M1 API**](md/DobotLinkHelp/6%20M1%20API) | M1 机器人 | **全量完整** | ✅ 已校验 | 包含队列控制、PTP、CP、圆弧插补及安全防护共 **35 个** API |
| [**7 CR API**](md/DobotLinkHelp/7%20CR%20API) | CR 协作机器人 | **全量完整** | ✅ 已校验 | 包含标定、安全配置、电子皮肤及轨迹复现等 **37 个** API |
| [**8 MagicianPro API**](md/DobotLinkHelp/8%20MagicianPro%20API) | Magician Pro 机械臂 | **全量完整** | ✅ 已校验 | 包含数据交换、传送带跟踪、Pro 特殊接口等 **24 个** API |
| [**9 MagicianGO API**](md/DobotLinkHelp/9%20MagicianGO%20API) | Magician GO 全向小车 | **全量完整** | ✅ 已校验 | 包含底盘控制、小车相机及 MagicBox 等共 **25 个** API |
| [**10 DebuggerLite API**](md/DobotLinkHelp/10%20DebuggerLite%20API) | DebuggerLite 调试器 | **全量完整** | ✅ 已校验 | 包含 `Prepare`、`Start`、`Wait` 及 `Stop` 等 **9 个** API |
| [**11 Download API**](md/DobotLinkHelp/11%20Download%20API) | 固件下载与更新 | **全量完整** | ✅ 已校验 | 包含固件升级、多系列固件获取与状态确认共 **10 个** API |
| [**13 错误码**](md/DobotLinkHelp/13%20错误码) | 错误码说明 | **全量完整** | ✅ 已校验 | 整理了 DobotLink 所有底层错误状态的对照表 |
| [**index.md**](md/DobotLinkHelp/index.md) | 全量 API 索引页 | **100% 映射** | ✅ 已校验 | 按字母顺序排列的 770+ 个 API 网页的直达索引 |

---

### 4. DobotLink API 接口文档 (英文版)

以下是 `md/DobotLinkHelp_EN/` 子目录下所有子目录及核心文件的状态：

| 子目录/文件名称 | 对应功能模块 | 内容完整度 | 校验状态 | 详细备注 / 统计数据 |
| :--- | :--- | :---: | :---: | :--- |
| [**1 Preface**](md/DobotLinkHelp_EN/1%20前言) | 前言与开发协议 | **全量完整** | ✅ 已校验 | 包含英文版接口协议说明等入门前置知识 |
| [**2 DobotLink API**](md/DobotLinkHelp_EN/2%20DobotLink%20API) | DobotLink 核心 API | **全量完整** | ✅ 已校验 | 包含 `CleanLogs`、`CloseDobotLink` 等 **12 个** 核心控制 API |
| [**3 Magician API**](md/DobotLinkHelp_EN/3%20Magician%20API) | Magician 机械臂 | **全量完整** | ✅ 已校验 | 包含 PTP、JOG、IO 及传送带等 **44 个** API |
| [**4 MagicianLite API**](md/DobotLinkHelp_EN/4%20MagicianLite%20API) | Magician Lite 机械臂 | **全量完整** | ✅ 已校验 | 包含点到位、滑轨、传送带、吸盘及通用 IO 共 **24 个** API |
| [**5 MagicBox API**](md/DobotLinkHelp_EN/5%20MagicBox%20API) | Magic Box 控制箱 | **全量完整** | ✅ 已校验 | 包含电机参数、滑轨、手持示教及多传感器共 **30 个** API |
| [**6 M1 API**](md/DobotLinkHelp_EN/6%20M1%20API) | M1 机器人 | **全量完整** | ✅ 已校验 | 包含队列控制、PTP、CP、圆弧插补及安全防护共 **35 个** API |
| [**7 CR API**](md/DobotLinkHelp_EN/7%20CR%20API) | CR 协作机器人 | **全量完整** | ✅ 已校验 | 包含标定、安全配置、电子皮肤及轨迹复现等 **37 个** API |
| [**8 MagicianPro API**](md/DobotLinkHelp_EN/8%20MagicianPro%20API) | Magician Pro 机械臂 | **全量完整** | ✅ 已校验 | 包含数据交换、传送带跟踪、Pro 特殊接口等 **24 个** API |
| [**9 MagicianGO API**](md/DobotLinkHelp_EN/9%20MagicianGO%20API) | Magician GO 全向小车 | **全量完整** | ✅ 已校验 | 包含底盘控制、小车相机及 MagicBox 等共 **25 个** API |
| [**10 DebuggerLite API**](md/DobotLinkHelp_EN/10%20DebuggerLite%20API) | DebuggerLite 调试器 | **全量完整** | ✅ 已校验 | 包含 `Prepare`、`Start`、`Wait` 及 `Stop` 等 **9 个** API |
| [**11 Download API**](md/DobotLinkHelp_EN/11%20Download%20API) | 固件下载与更新 | **全量完整** | ✅ 已校验 | 包含固件升级、多系列固件获取与状态确认共 **10 个** API |
| [**13 Error Code**](md/DobotLinkHelp_EN/13%20Error%20Code) | 错误码说明 | **全量完整** | ✅ 已校验 | 整理了 DobotLink 英文版所有底层错误状态的对照表 |
| [**index.md**](md/DobotLinkHelp_EN/index.md) | 全量 API 索引页 | **100% 映射** | ✅ 已校验 | 按字母顺序排列的 770+ 个 API 网页的直达索引 |
| [**README.md**](md/DobotLinkHelp_EN/README.md) | 英文版导航首页 | **100% 映射** | ✅ 已校验 | 英文版接口文档的结构总引导页 |

---

## 🛠️ 校验方式与可信度说明

1.  **全量单页面爬取**：
    编写专用清洗爬虫下载了 **183 个 Python 详细开发网页**，保证 API 信息 100% 覆盖。
2.  **HTML 到 Markdown 的格式化转换**：
    基于自定义 Python `HTMLParser` 转换引擎，将原始 HTML 的排版转换为无损 Markdown 标题和代码块，彻底清除了 GitBook 背景脚本噪音。
3.  **便携性与相对路径**：
    整套文档所有的内部跳转以及根目录 README 关联均采用**相对路径链接**，完美支持在任何机器、Git 托管平台或静态网站中无缝阅读与跳转。

---

## 📝 更新与修复记录 (Changelog)

### 2026-05-26
- **补齐缺失 API 文档**：
  - 新增 `dobotlink.MagicianGO.SetTraceLoop` 接口的中文与英文文档：[中文版](md/DobotLinkHelp/9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetTraceLoop.md) 和 [英文版](md/DobotLinkHelp_EN/9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetTraceLoop.md)（原官方 CHM 文档库中缺失该接口）。
  - 在中英文版 API 全量索引页 [index.md](md/DobotLinkHelp/index.md) 和 [index.md](md/DobotLinkHelp_EN/index.md) 中添加了对应的字母索引链接。
- **修复英文版 API 接口笔误**：
  - **`ConnectDobot` 接口**：将错误的 method 路径 `dobotlink.MagicianPro.ConnectDobot` 修正为正确的 `dobotlink.MagicianGO.ConnectDobot`（文件：[ConnectDobot.md](md/DobotLinkHelp_EN/9%20MagicianGO%20API/9.1%20%E8%AE%BE%E5%A4%87%E8%BF%9E%E6%8E%A5(connect)/ConnectDobot.md)）。
  - **`SetRunningMode` 接口**：将参数 `runningState` 修正为正确的 `runningMode`（文件：[SetRunningMode.md](md/DobotLinkHelp_EN/9%20MagicianGO%20API/9.4%20%E5%BA%95%E7%9B%98%E6%8E%A7%E5%88%B6(control)/SetRunningMode.md)）。
