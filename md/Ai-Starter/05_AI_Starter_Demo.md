# AI-Starter Demo

## 6. AI-Starter Demo

### 6.1 自动巡线 Demo

#### 6.1.1 介绍

      该Demo实现了AI-Starter在地图上自动巡线功能。

#### 6.1.2 操作步骤

      步骤 1             开机后，电机停止。
      步骤 2             按下“启动|停止”按键，发出“滴一声”后开始巡线。
      步骤 3             再次按下“启动|停止”按键，发出“滴一声”后停止巡线。

#### 6.1.3 关键代码说明

      1) 获取当前巡线传感器值。

##### **程序 6.1 获取传感器数值**

```cpp

void getCurrentIRState(int *irstate)

{

- irstate = 0;

      for (int i = 0; i < IR_NUM; i++) {

- irstate |= AIStarter_SmartBotGetIRModuleValue(i) << i;

      }

}

```

      2) 获取当前小车姿态。

##### **程序 6.2 获取小车姿态**

```cpp

float getCurrentPos(const int irstate)

{

      const float coeff = 0.7;

      const int irPos[] = {-30, -18, -6, 6, 18, 30};//设置各个红外对管权重值

      static float lastPos;

      float curPos;

      float readPos;

      int total = 0;

      int irOffCnt = 0;

      //calculate the car position offset

    for (int i = 0; i < IR_NUM; i++) {

         if (irstate & (1 << i)) {

               total += irPos[i];

               irOffCnt++;

         }

    }

    if (irOffCnt) {

         readPos = total / irOffCnt;

    }

    else {

         readPos = lastPos;

    }

    //calculate the current position

    curPos = (1 - coeff) * lastPos + coeff * readPos;

    lastPos = curPos;

    return curPos;

}

```

     3) 设置小车速度。

##### **程序 6.3 设置小车速度**

```cpp

void setCarSpeed(const float curPos)

{

    const int baseSpeed = 50; //rpm

    const float kp = 1;

    const float ki = 0.06;

    const float kd = 0.0;

    const float errorsumLimit = 50;

    float error = curPos;

    static float lastError;

    static float errorsum;

    float errorChange;

    int speedLeftWheel;

    int speedRightWheel;

    int speedOffset;

      //pid

      errorsum += error;

      if (errorsum > errorsumLimit) {

              errorsum = errorsumLimit;

      }

      else if (errorsum < -errorsumLimit){

              errorsum = -errorsumLimit;

      }

      errorChange = error - lastError;

      speedOffset = kp * error + ki * errorsum + kd * errorChange;

      lastError = error;

      //calculate the wheel speed

      speedLeftWheel       = baseSpeed + speedOffset;

      speedRightWheel = baseSpeed - speedOffset;

      AIStarter_SmartBotSetMotor(MOTORL, speedLeftWheel);

      AIStarter_SmartBotSetMotor(MOTORR, speedRightWheel);

      Serial.println("go ahead");

}

```

### 6.2 自动避障 Demo

#### 6.2.1 介绍

      该Demo实现了AI-Starter自主避障功能。

#### 6.2.2 操作步骤

      步骤 1           开机后，电机停止。
      步骤 2           按下【启动|停止】
                             ，开始后开始避障。
      步骤 3           小车遇到障碍物后退一段距离，根据超声波传感器进行判断左转或右转，然后
                     继续前进。
      步骤 4           再次按下【启动|停止】按键，发出“滴一声”响后停止巡线。

#### 6.2.3 关键代码说明

      1) 初始化 AI-Starter。

##### **程序 6.4 初始化小车**

```cpp

AIStarter_SmartBotInit();

```

     2) 将 AI-Starter 超声波模块获取到的数据传入数组“dis”中。

##### **程序 6.5 保存超声波数据**

```cpp

dis[0] = AIStarter_SmartBotGetSonar(SONAR1);

dis[1] = AIStarter_SmartBotGetSonar(SONAR2);

dis[2] = AIStarter_SmartBotGetSonar(SONAR3);

```

     3) 根据超声波模块检测到障碍物的距离设置转向模式。

##### **程序 6.6 设置转向模式**

```cpp

     if(dis[0] > 2*DIS ){

          motorStatus = AHEAD;

     }else if(dis[0] > DIS    && dis[0] < 2*DIS ){

          motorStatus = motorStatus;

     }else if(dis[0] > 0    && dis[0] < DIS ){

          motorStatus = BACKRIGHT;

          break;

     }

     if(dis[1] > 2*DIS ){

          motorStatus = AHEAD;

     }else if(dis[1] > DIS    && dis[1] < 2*DIS ){

          motorStatus = motorStatus;

     }else if(dis[1] > 0    && dis[1] < DIS ){

          motorStatus = BACKRIGHT;

          break;

}

if(dis[2] > 2*DIS ){

          motorStatus = AHEAD;

     }else if(dis[2] > DIS    && dis[2] < 2*DIS ){

          motorStatus = motorStatus;

     }else if(dis[2] > 0    && dis[2] < DIS ){

          motorStatus = BACKLEFT;

          break;

                   }

```

      4) 根据超声波检测到障碍物的位置进行相应的转向，BACKRIGHT 为向右转，

            BACKLEFT 为向左转，AHEAD 为直行。

##### **程序 6.7 根据障碍物位置进行转向**

```cpp

      switch(motorStatus){

          case BACKRIGHT:

               AIStarter_SmartBotSetMotor(MOTORR,BACKSPEED);

               AIStarter_SmartBotSetMotor(MOTORL,BACKSPEED);

               delay(BACKTIME);

               AIStarter_SmartBotSetMotor(MOTORR,DIFSPEED);

               AIStarter_SmartBotSetMotor(MOTORL,FRONTSPEED);

               delay(SWERVETIME);

          break;

          case BACKLEFT:

               AIStarter_SmartBotSetMotor(MOTORR,BACKSPEED);

               AIStarter_SmartBotSetMotor(MOTORL,BACKSPEED);

               delay(BACKTIME);

               AIStarter_SmartBotSetMotor(MOTORR,FRONTSPEED);

               AIStarter_SmartBotSetMotor(MOTORL,DIFSPEED);

               delay(SWERVETIME);

          break;

          case AHEAD:

               AIStarter_SmartBotSetMotor(MOTORR,FRONTSPEED);

               AIStarter_SmartBotSetMotor(MOTORL,FRONTSPEED);

          break;

          default:

          break;

}

```

### 6.3 白平衡校准 Demo

#### 6.3.1 介绍

      AI-Starter颜色传感器校准白平衡。

#### 6.3.2 操作步骤

      步骤 1      将AI-Starter放在A4白纸上。
      步骤 2      按下“启动|停止”开关，自动校准白平衡值。

#### 6.3.3 关键代码说明

      1)   初始化AI-Starter。

##### **程序 6.8 初始化 AI-Starter**

```cpp

AIStarter_SmartBotInit();

```

      1) 校准白平衡。

##### **程序 6.9 校准白平衡**

```cpp

AIStarter_SmartBotSetColorWB(COLORSENOR1);

AIStarter_SmartBotSetColorWB(COLORSENOR2);

```

### 6.4 颜色识别与自动巡线 Demo

#### 6.4.1 介绍

           该Demo实现了AI-Starter颜色识别结合巡线使用的功能。

#### 6.4.2 操作步骤

      步骤 1      按下“启动|停止”按键，发出“滴一声”响后进行巡线。
      步骤 2      巡线过程中，检测到黑色停止线后小车停止运动，并开始检测颜色。
      步骤 3      识别颜色为红色时，小车停留3秒，同时“滴滴滴”响三声。
      步骤 4      识别颜色为绿色时，小车停留3秒，蜂鸣器长鸣3秒。
      步骤 5      完成上述任务后，继续前进。
      步骤 6      再次按下“启动|停止”按键，发出“滴一声”响后停止巡线。

#### 6.4.3 关键代码说明

      1) 初始化 AI-Starter。

##### **程序 6.10   初始化小车**

```cpp

AIStarter_SmartBotInit();

```

      2) 检测颜色。

##### **程序 6.11 检测颜色**

```cpp

if(AIStarter_SmartBotGetColorSenor(COLORSENOR1,RCOLOR)
- AIStarter_SmartBotGetColorSenor(COLORSENOR1,GCOLOR) > 30 &&

        AIStarter_SmartBotGetColorSenor(COLORSENOR1,RCOLOR)
- AIStarter_SmartBotGetColorSenor(COLORSENOR1,BCOLOR) > 30) {

              colorState = RLINE;

}

```

         3) 根据颜色状态进行相应动作。

##### **程序 6.12   根据颜色执行动作**

```cpp

        switch(colorState) {

            case OTHERLINE:

                   //colorRec = false;

                   lineState = LINEPATROL;

            break;

            case RLINE:

                   delay(3000);

                   //colorRec = false;

                   lineState = LINEPATROL;

            break;

            case GLINE:

                   delay(3000);

                   //colorRec = false;

                   lineState = LINEPATROL;

            break;

            default:

            break;

    }

```

### 6.5 机械臂协作 Demo

#### 6.5.1 介绍

              该Demo实现AI-Starter与Magician协作。
              1)     AI-Starter到达绿线停止一分钟。
              2)     机械臂通过Pixy摄像头检测到小车到达搬运点后开始执行搬运动作。
              3)     机械臂从方块区吸取方块放置到小车上。
              4)     一分钟后AI -Starter装载完毕重新启动巡线。

#### 6.5.2 操作步骤

    AI-Starter
      步骤 1       按下“启动|停止”按键，发出“滴一声”响后进行巡线。
      步骤 2       巡线过程中，检测到黑色停止线后小车停止运动，并开始检测颜色。
      步骤 3       识别颜色为红色时，小车停留3秒，同时“滴滴滴”响三声。
      步骤 4       识别颜色为绿色时，发出“滴一声”
                                ，小车停留1分钟。
      步骤 5       完成上述任务后，继续前进。
      步骤 6       再次按下“启动|停止”按键，发出“滴一声”响后停止巡线。
    Magician
      步骤 1       打开Magician Cooperation文件夹下的Magician文件夹，上传Magician固件至
                 Arduino拓展板。
      步骤 2       当机械臂检测到AI-Starter停至装载区时，开始执行装载方块任务。
      步骤 3       AI-Starter继续巡线。

#### 6.5.3 关键代码说明

    AI-Starter

      1) 初始化 AI-Starter。

##### **程序 6.13    初始化小车**

```cpp

AIStarter_SmartBotInit();

```

      2) 检测颜色。

##### **程序 6.14    检测颜色**

```cpp

if(AIStarter_SmartBotGetColorSenor(COLORSENOR1,RCOLOR)
- AIStarter_SmartBotGetColorSenor(COLORSENOR1,GCOLOR) > 30 &&

    AIStarter_SmartBotGetColorSenor(COLORSENOR1,RCOLOR)
- AIStarter_SmartBotGetColorSenor(COLORSENOR1,BCOLOR) > 30) {

           colorState = RLINE;

}

```

      3) 根据颜色状态进行相应动作。

##### **程序 6.15    根据颜色执行动作**

```cpp

     switch(colorState) {

         case OTHERLINE:

                 //colorRec = false;

                 lineState = LINEPATROL;

            break;

            case RLINE:

                 delay(3000);

                 //colorRec = false;

                 lineState = LINEPATROL;

            break;

            case GLINE:

                 delay(3000);

                 //colorRec = false;

                 lineState = LINEPATROL;

            break;

            default:

            break;

     }

```

Magician
         1） 设置方块点位。

##### **程序 6.16   设置方块点位**

```cpp

float AreaPoint[4][3] = {

     {137.05, -206.94, -39},

     {137.05, -244.31, -39},

     {100.50, -206.94, -39},

     {100.50, -244.31, -39}

};
```

         2） 设置AI-Starter装载点位。

##### **程序 6.17   设置装载点位**

```cpp

float trayPoint[4][3] = {

     {308.12,   25.92, 28},

     {308.12, -15.92,   28},

     {258.12,   25.92, 28},

     {258.12, -15.92,   28}

};

```

         3） 吸取方块，放置AI-Starter装载点位。

##### **程序 6.18      吸取方块**

```cpp

void AreaToAIStarter()

{

      for(uint8_t i=0; i<4; i++){

           Dobot_SetPTPCmdEx(JUMP_XYZ, AreaPoint[i][0], AreaPoint[i][1], AreaPoint[i][2], 0);

           Dobot_SetEndEffectorSuctionCupEx(true);

           Dobot_SetPTPCmdEx(MOVL_XYZ, AreaPoint[i][0], AreaPoint[i][1], AreaPoint[i][2]+70, 0);

           Dobot_SetPTPCmdEx(JUMP_XYZ, trayPoint[i][0], trayPoint[i][1], trayPoint[i][2], 0);

           Dobot_SetEndEffectorSuctionCupEx(false);

           Dobot_SetPTPCmdEx(MOVL_XYZ, trayPoint[i][0], trayPoint[i][1], trayPoint[i][2]+30, 0);

      }

      Dobot_SetPTPCmdEx(MOVJ_XYZ, InitPositionX, InitPositionY, InitPositionZ, InitPositionR);

}

```

      4） 初始化摄像头和机械臂。

##### **程序 6.19      初始化摄像头和机械臂**

```cpp

pixy.init();

Dobot_Init();

```

      5） 检测物块数量。

##### **程序 6.20      检测物块数量**

```cpp

pixy.ccc.getBlocks();

```

### 6.6 舵机驱动 Demo

#### 6.6.1 介绍

      AI-Starter舵机驱动示例。

#### 6.6.2 操作步骤

      步骤 1        将舵机接入AI-Starter数字 I/O 7。I/O 7说明请参照章节3.1.1概述。
      步骤 2        按下“启动|停止”开关，舵机自动往复旋转180°。

#### 6.6.3 关键代码说明

      1)       初始化AI-Starter。

##### **程序 6.21       初始化 AI-Starter**

```cpp

      AIStarter_SmartBotInit();

      AIStarter_SmartBotServoAttach(SERVO1);

```

      2) 舵机做 180°往复运动。

##### **程序 6.22    舵机往复运动**

```cpp

for (pmwServo = 0; pmwServo <= 180; pmwServo += 1) {

      AIStarter_Servo.write(pmwServo);

      delay(15);

}

for (pmwServo = 180; pmwServo >= 0; pmwServo -= 1) {

      AIStarter_Servo.write(pmwServo);

      delay(15);

}

```

### 6.7 Xbee 通信 Demo

#### 6.7.1 介绍

      AI-Starter与PC端Xbee通信示例。

#### 6.7.2 操作步骤

      步骤 1         在XCTU官网https://www.digi.com/support/productdetail?pid=3352&type=utilities
                   下载XCTU软件。
      步骤 2         使用XCTU软件烧录XbeeMatch.xpro固件。
      步骤 3         烧录完成后，将Xbee装回AI-Starter串口2上，串口2请参考章节3.1.1概述。
      步骤 4         按下“启动|停止”开关，使用XCTU给AI-Starter发送控制命令。
      步骤 5         根据PC端发送的命令，AI-Starter执行相应的动作。

#### 6.7.3 关键代码说明

      1)   初始化AI-Starter。

##### **程序 6.23    初始化 AI-Starter**

```cpp

AIStarter_SmartBotInit();

```

      2) 读取 Xbee 信息。

##### **程序 6.24    读取 Xbee 信息**

```cpp

strCommand = AIStarter_SmartBotXbeeRead();

```

     3)   根据Xbee信息执行相应动作

##### **程序 6.25    根据 Xbee 信息执行相应动作**

```cpp

if(!AIStarter_SmartBotXbeeCompare(strCommand, "Ahead")) {

     rOffSet = 1;

     lOffSet = 1;

} else if(!AIStarter_SmartBotXbeeCompare(strCommand, "Back")) {

     rOffSet = -1;

     lOffSet = -1;

} else if(!AIStarter_SmartBotXbeeCompare(strCommand, "TurnLeft")) {

     rOffSet = 1;

     lOffSet = 0.5;

} else if(!AIStarter_SmartBotXbeeCompare(strCommand, "TurnRight")) {

     rOffSet = 0.5;

     lOffSet = 1;

} else if(!AIStarter_SmartBotXbeeCompare(strCommand, "Stop")) {

     rOffSet = 0;

     lOffSet = 0;

}

```

     4)   清除Xbee信息

##### **程序 6.26      清除 Xbee 信息**

```cpp

AIStarter_SmartBotXbeeClear();

```
