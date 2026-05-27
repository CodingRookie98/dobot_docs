# API 接口说明

## 7.1 初始化 (AIStarter_SmartBotInit)
- 原型：
  ```cpp
  int AIStarter_SmartBotInit ()
  ```
- 描述：初始化
- 参数：无
- 返回：无
---
## 7.2 设置小车速度 (AIStarter_SmartBotSetMovment)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetMovment (int dir, int speed)
  ```
- 描述：设置小车速度和方向
- 参数：
  - dir：设置小车方向
      ```cpp
        enum{
        FRONT,
        BACK,
        RIGHT,
        LEFT
        }
      ```;
  - speed：设置占空比，范围：0~255
- 返回：无
---
## 7.3 设置小车运动方向/速度/时间 (AIStarter_SmartBotSetMovmentTime)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetMovmentTime (int dir, int speed,float time)
  ```
- 描述：设置小车运动方向、速度和时间
- 参数：
  - dir：设置小车方向
      ```cpp
        enum {
        FRONT,
        BACK,
        RIGHT,
        LEFT
        }
      ```;
  - speed：设置占空比，范围：0~255
  - time：设置小车运动时间（单位：s）
- 返回：无
---
## 7.4 设置电机转速 (AIStarter_SmartBotSetMotor)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetMotor(int port, int speed)
  ```
- 描述：设置电机转速
- 参数：
  - port：选择电机
      ```cpp
        enum {
        MOTORR,
        MOTORL
        }
      ```;
  - speed：设置电机转速。范围：0~200rpm
- 返回：无
---
## 7.5 设置电机参数 (AIStarter_SmartBotSetMotorPI)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetMotorPI (float KP, float KI)
  ```
- 描述：设置电机参数
- 参数：
  - KP：比例因子。取值范围：0.5~2.5
  - KI：积分因子。取值范围：0.05~0.5
- 返回：无
---
## 7.6 获取电机位姿 (AIStarter_SmartBotGetMotorPose)
- 原型：
  ```cpp
  float AIStarter_SmartBotGetMotorPose (int port)
  ```
- 描述：获取电机位姿
- 参数：
  - port：选择电机
      ```cpp
        enum {
        MOTORR,
        MOTORL
        }
      ```;
- 返回：电机编码器读数
---
## 7.7 初始化超声波传感器 (AIStarter_SmartBotSetSonar)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetSonar (int port)
  ```
- 描述：初始化超声波传感器
- 参数：
  - port：选择超声波
      ```cpp
        enum {
        SONAR1,
        SONAR2,
        SONAR3
        }
      ```;
- 返回：无
---
## 7.8 获取超声波探测距离 (AIStarter_SmartBotGetSonar)
- 原型：
  ```cpp
  float AIStarter_SmartBotGetSonar (int port)
  ```
- 描述：获取超声波传感器探测的距离
- 参数：
  - port：选择超声波传感器
      ```cpp
        enum {
        SONAR1,
        SONAR2,
        SONAR3
        }
      ```;
- 返回：超声波探测到障碍物距小车的距离（单位：cm）
---
## 7.9 探测障碍物 (AIStarter_SmartBotGetBarrier)
- 原型：
  ```cpp
  bool AIStarter_SmartBotGetBarrier (int port)
  ```
- 描述：探测前方是否有障碍物
- 参数：
  - port：选择超声波传感器
      ```cpp
        enum {
        SONAR1,
        SONAR2,
        SONAR3
        }
      ```;
- 返回：1：检测到障碍物；0：未检测到障碍物
---
## 7.10 获取巡线数据 (AIStarter_SmartBotGetIRModuleValue)
- 原型：
  ```cpp
  int AIStarter_SmartBotGetIRModuleValue (int port)
  ```
- 描述：获取巡线数据
- 参数：
  - port：选择巡线传感器端口
      ```cpp
        enum {
        IR1,
        IR2,
        IR3,
        IR4,
        IR5,
        IR6
        }
      ```;
- 返回：1：检测到黑线；0：未检测到黑线
---
## 7.11 获取地磁角度 (AIStarter_SmartBotGetCompass)
- 原型：
  ```cpp
  float AIStarter_SmartBotGetCompass ()
  ```
- 描述：获取地磁角度
- 参数：无
- 返回：获取地磁角度
---
## 7.12 地磁校准 (AIStarter_SmartBotSetCompassCalibration)
- 原型：
  ```cpp
  void AIStarter_SmartBotSetCompassCalibration()
  ```
- 描述：校准方法：开机后按下最左侧按钮开始校准，校准过程中使小车在空间内分别绕XYZ三
轴方向旋转360°以上，旋转完成后按下最左侧按钮结束校准
- 参数：无
- 返回：地磁校准
---
## 7.13 设置颜色白平衡 (AIStarter_SmartBotSetColorWB)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetColorWB (int port)
  ```
- 描述：设置颜色白平衡
- 参数：
  - port：选择颜色传感器
      ```cpp
        enum{
        COLORSENOR1,
        COLORSENOR2
        }
      ```;
- 返回：无
---
## 7.14 启停颜色传感器 (AIStarter_SmartBotSetColorSenor)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetColorSenor (int port,bool ison)
  ```
- 描述：控制颜色传感器的启停
- 参数：
  - port：选择颜色传感器
      ```cpp
        enum{
        COLORSENOR1,
        COLORSENOR2
        }
      ```;
  - ison：true 开启；false 关闭
- 返回：无
---
## 7.15 检测颜色 (AIStarter_SmartBotDetColorSenor)
- 原型：
  ```cpp
  bool AIStarter_SmartBotDetColorSenor (int port,int color)
  ```
- 描述：检测所选的对应颜色即红绿蓝是否存在
- 参数：
  - port：选择颜色传感器
      ```cpp
        enum{
        COLORSENOR1,
        COLORSENOR2
        }
      ```;
  - color：选择所检测的颜色
  enum{
  RCOLOR,
  GCOLOR,
  BCOLOR,
  };
- 返回：1：检测到颜色；0：未检测到颜色
---
## 7.16 获取 RGB 色值 (AIStarter_SmartBotGetColorSenor)
- 原型：
  ```cpp
  int AIStarter_SmartBotGetColorSenor (int port, int color)
  ```
- 描述：获取RGB色值
- 参数：
  - port：选择颜色传感器
      ```cpp
        enum{
        COLORSENOR1,
        COLORSENOR2
        }
      ```;
  - color：选择颜色滤波器
  enum{
  RCOLOR,
  GCOLOR,
  BCOLOR,
  };
- 返回：返回RGB色值，范围：0~255
---
## 7.17 初始化按键 (MobilePlatform_SmartBotSetKeyInit)
- 原型：
  ```cpp
  int MobilePlatform_SmartBotSetKeyInit()
  ```
- 描述：初始化按钮
- 参数：无
- 返回：无
---
## 7.18 获取按键状态 (AIStarter_SmartBotGetKeyValue)
- 原型：
  ```cpp
  int AIStarter_SmartBotGetKeyValue (int key)
  ```
- 描述：设置按键
- 参数：
  - key：选择按键
      ```cpp
        enum{
        SW1,
        SW2,
        SW3
        }
      ```;
- 返回：1：按键按下；0：按键释放
---
## 7.19 设置灯光状态 (MobilePlatform_SmartBotSetLED)
- 原型：
  ```cpp
  int MobilePlatform_SmartBotSetLED(int port, int state)
  ```
- 描述：设置LED灯
- 参数：
  - port：选择 LED 灯。
      ```cpp
        enum{
        LED1,
        LED2
        }
      ```;
  - state：设置状态。
  enum{
  ON,
  OFF,
  BLINK
  };
- 返回：无
---
## 7.20 获取光敏数值 (AIStarter_SmartBotGetLightAnalog)
- 原型：
  ```cpp
  int AIStarter_SmartBotGetLightAnalog ()
  ```
- 描述：获取光敏传感器数值
- 参数：无
- 返回：光敏传感器数值
---
## 7.21 设置超声波传感器检测距离 (AIStarter_SmartBotSetSonarThreshold)
- 原型：
  ```cpp
  int AIStarter_SmartBotSetSonarThreshold (int dis)
  ```
- 描述：设置超声波传感器检测距离
- 参数：
  - dis：设置检测距离。(单位：cm)
- 返回：无
---
## 7.22 连接舵机 (AIStarter_SmartBotServoAttach)
- 原型：
  ```cpp
  int AIStarter_SmartBotServoAttach(int servo)
  ```
- 描述：连接舵机
- 参数：
  - servo：选择舵机
      ```cpp
        enum{
        SERVO1,
        SERVO2
        }
      ```;
- 返回：无
---
## 7.23 设置舵机角度 (AIStarter_SmartBotServoWrite)
- 原型：
  ```cpp
  int AIStarter_SmartBotServoWrite(int servo, int value)
  ```
- 描述：设置舵机角度
- 参数：
  - servo：选择舵机
      ```cpp
        enum{
        SERVO1,
        SERVO2
        }
      ```;
  - value：设置舵机角度，取值范围：0°~180°
- 返回：无
---
## 7.24 断开舵机连接 (AIStarter_SmartBotServoDetach)
- 原型：
  ```cpp
  int AIStarter_SmartBotServoDetach(int servo)
  ```
- 描述：断开舵机连接
- 参数：
  - 选择舵机：
      ```cpp
        enum{
        SERVO1,
        SERVO2
        }
      ```;
- 返回：无
---
## 7.25 开启后台定时器任务 (AIStarter_SmartBotTimerTaskAttach)
- 原型：
  ```cpp
  int AIStarter_SmartBotTimerTaskAttach()
  ```
- 描述：开启定时器任务
- 参数：无
- 返回：无
---
## 7.26 关闭后台定时器任务 (AIStarter_SmartBotTimerTaskDetach)
- 原型：
  ```cpp
  int AIStarter_SmartBotTimerTaskDetach()
  ```
- 描述：关闭定时器任务
- 参数：无
- 返回：无
---
## 7.27 Xbee 数据读取 (AIStarter_SmartBotXbeeRead)
- 原型：
  ```cpp
  String& AIStarter_SmartBotXbeeRead()
  ```
- 描述：读取Xbee数据
- 参数：无
- 返回：无
---
## 7.28 Xbee 数据写入 (AIStarter_SmartBotXbeeWrite)
- 原型：
  ```cpp
  String& AIStarter_SmartBotXbeeWrite()
  ```
- 描述：Xbee数据写入
- 参数：无
- 返回：无
---
## 7.29 Xbee 数据对比 (AIStarter_SmartBotXbeeCompare)
- 原型：
  ```cpp
  int AIStarter_SmartBotXbeeCompare(const String &str1, const String &str2)
  ```
- 描述：对比两个字符串
- 参数：无
- 返回：非0表示字符串不相同
---
## 7.30 Xbee 数据清除 (AIStarter_SmartBotXbeeClear)
- 原型：
  ```cpp
  int AIStarter_SmartBotXbeeClear()
  ```
- 描述：清除Xbee数据
- 参数：无
- 返回：无
---
