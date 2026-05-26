# Dobot Magician 机械臂接口指令


                            

    
    
                                
                                
                                
## 3.6 Dobot Magician


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 点到点运动

- 
原型：

```python
magician.ptp(mode,x,y,z,r)

```

- 
描述：机械臂以设定的模式运动至目标点。

- 
必选参数：

  - mode：PTP 模式，取值范围：0~9，具体含义如下：

    - 0：JUMP 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 1：MOVJ 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 2：MOVL 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 3：JUMP 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 4：MOVJ 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 5：MOVL 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 6：MOVJ 模式，（x,y,z,r）为关节坐标系下的坐标增量；

    - 7：MOVL 模式，（x,y,z,r）为笛卡尔坐标系下的坐标增量；

    - 8：MOVJ 模式，（x,y,z,r）为笛卡尔坐标系下的坐标增量；

    - 9：JUMP 模式，平移时运动模式为 MOVL。（x,y,z,r）为笛卡尔坐标系下的坐标增量。

  - x：x 坐标值。

  - y：y 坐标值。

  - z：z 坐标值。

  - r：r 坐标值。

- 返回：

  - True： 指令完成。

  - False：指令未完成。

- 
示例

```python
magician.ptp(mode=0, x=200, y=100, z=10, r=0)

```

以JUMP 模式，在笛卡尔坐标系下运动到(200,100,10,0)。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置滑轨开关及版本

- 
原型：

```python
magician.set_device_withl(enable, version)

```

- 
描述：设置滑轨的开关状态以及版本。

- 
必选参数：

  - enable：使能滑轨，True：使能；False：未使能。

  - version：滑轨版本号。0：V1 版本；1：V2 版本，根据实际连接方式选择。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_device_withl(enable=True, version=0)

```

滑轨上使能，并设置滑轨版本为V1 版本。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 滑轨点到点运动速度比例

- 
原型：

```python
magician.set_ptpl_params(vel, accel)

```

- 
描述：设置滑轨的速度和加速度。

- 
必选参数：

  - vel：滑轨的速度比例，取值范围：1~100。

  - version：滑轨的加速度比例，取值范围：1~100。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_ptpl_params(vel=50, accel=50)

```

设置滑轨的速度比例为50%，加速度比例为50%。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 点到点运动（包含滑轨）

- 
原型：

```python
magician.set_ptpwithl_cmd(mode, x, y, z, r, l)

```

- 
描述：执行带滑轨的点到点运动。

- 
必选参数：

  - mode：PTP 模式，取值范围：0~9，具体含义如下：

    - 0：JUMP 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 1：MOVJ 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 2：MOVL 模式，（x,y,z,r）为笛卡尔坐标系下的目标点坐标；

    - 3：JUMP 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 4：MOVJ 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 5：MOVL 模式，（x,y,z,r）为关节坐标系下的目标点坐标；

    - 6：MOVJ 模式，（x,y,z,r）为关节坐标系下的坐标增量；

    - 7：MOVL 模式，（x,y,z,r）为笛卡尔坐标系下的坐标增量；

    - 8：MOVJ 模式，（x,y,z,r）为笛卡尔坐标系下的坐标增量；

    - 9：JUMP 模式，平移时运动模式为 MOVL。（x, y, z, r）为笛卡尔坐标系下的坐标增量。

  - x：x 坐标值。

  - y：y 坐标值。

  - z：z 坐标值。

  - r：r 坐标值。

  - l：滑轨位姿的坐标值。

- 
返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_ptpwithl_cmd(mode=1, x=200, y=100, z=10, r=0, l=100)

```


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置R轴角度

- 
原型：

```python
 magician.set_r(r)

```

- 
描述：设置R轴的角度。

- 
必选参数：

  - r：R 轴角度值，单位：°。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_r(r=100)

```

设置R 轴的角度为100°。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置运动速度比例

- 
原型：

```python
magician.motion_params = vel, acc

```

- 
描述：设置运动速度和加速度。

- 
必选参数：

  - vel：速度的比例。

  - acc：加速度的比例。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.motion_params = 50, 50

```

设置运动速度的比例为50%，加速度的比例为50%。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置门型运动参数

- 
原型：

```python
magician.jump_params = zlimit, height

```

- 
描述：设置门型运动参数。

- 
必选参数：

  - zlimit：最大抬升高度；

  - height：抬升高度。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.jump_params = 100, 20 # zlimit, height

```

设置门型运动参数，其中，最大抬升高度为100mm，抬升高度20mm。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置 IO 端口模式

- 
原型：

```python
magician.set_multiplexing(io, multiplex)

```

- 
描述：设置 IO 端口模式。

- 
必选参数：

  - io：io 端口序号，数据类型：str，取值范围："DO_01"~"DO_20"。

  - multiplex：io 端口模式，取值范围 0-6，具体如下：

    - 0：IOFunctionDummy，不配置功能；

    - 1：IOFunctionDO，IO 输出；

    - 2：IOFunctionPWM，PWM 输出；

    - 3：IOFunctionDI，IO 输入；

    - 4：IOFunctionADC，AD 输入；

    - 5：IOFunctionDIPU，上拉输入；

    - 6：IOFunctionDIPD，下拉输入。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_multiplexing(io="DO_01", multiplex=1)

```

设置“DO_01”端口的模式为IO 输出。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置PWM输出端口频率及占空比

- 
原型：

```python
magician.set_pwm(io, freq, cycle)

```

- 
描述：设置 PWM 输出端口的频率及占空比。

- 
必选参数：

  - io：io 端口序号，数据类型：str，取值范围："DO_01"~"DO_20"。

  - freq：PWM 频率，范围：10Hz-1MHz。

  - cycle：占空比，范围：0-100。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_pwm(io="DO_01", freq=10, cycle=30)

```

设置“DO_01”端口的PWM 频率为10Hz，其占空比为30%。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置数字输出端口

- 
原型：

```python
magician.set_do(io，level)

```

- 
描述：设置数字端口输出的电平。

- 
必选参数：

  - io：io 端口序号，数据类型：str，取值范围："DO_01"~"DO_20"。

  - level：输出电平，0：低电平，1：高电平。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_do(io="DO_01", level=1)

```

设置“DO_01”端口为高电平输出。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取数字信号

- 
原型：

```python
magician.get_di(io)

```

- 
描述：获取IO接口的数字信号。

- 
必选参数：  

  - io：io 端口序号，数据类型：str，取值范围："DI_01"~"DI_20"。

- 
返回：

  - 0： 低电平。

  - 1： 高电平。

- 
示例

```python
magician.get_di(io="DI_01")

```

获取“DI_01”端口的数字信号(高电平或低电平)。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取模拟信号

- 
原型：

```python
magician.get_adc(io)

```

- 
描述：获取IO接口的模拟信号。

- 
必选参数：  

  - io：io 端口序号，数据类型：str，取值范围："DO_01"~"DO_20"。

- 
返回：  

  - val：模拟信号，取值范围：0-4095。

- 
示例

```python
magician.get_adc(io="DO_01")

```

获取“DO_01”端口的模拟信号。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置末端吸盘

- 
原型：

```python
magician.set_endeffector_suctioncup(enable, on)

```

- 
描述：设置吸盘的工作状态。

- 
必选参数：

  - enable：吸盘使能状态。True：吸盘使能；False：吸盘未使能。

  - on：控制吸盘吸取或释放。True：吸盘吸取；False：吸盘释放。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_endeffector_suctioncup(enable=True, on=True)

```

吸盘上使能，并且吸盘进行吸取操作。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置末端手爪

- 
原型：

```python
magician.set_endeffector_gripper(enable, on)

```

- 
描述：设置手爪的工作状态。

- 
必选参数：

  - enable：手爪使能状态。True：手爪使能；False：手爪未使能。

  - on：控制夹爪抓取或释放。True：夹爪抓取；False：夹爪释放。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_endeffector_gripper(enable=True, on=True)

```

手爪上使能，并且手爪进行抓取操作。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置光电传感器

- 
原型：

```python
magician.set_infrared_sensor(port, enable, version)

```

- 
描述：设置光电传感器使能状态及版本。

- 
必选参数：

  - port：光电传感器连接至 Magician的端口，取值范围：1，2，4，5。其中，port 1，port 2，port 4，port 5分别对应Magician的GP1，GP2，GP4，GP5。

  - enable：使能光电传感器。True：使能；False：未使能。

  - version：光电传感器版本。0：V1.0；1：V2.0。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_infrared_sensor(port=1, enable=True, version=1)

```

光电传感器与Magician的端口1连接，控制光电传感器上使能，并设置其版本为V2.0。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取光电传感器读数

- 
原型：

```python
magician.get_infrared_sensor(port)

```

- 
描述：获取光电传感器的返回值。

- 
必选参数：  

  - port：光电传感器连接至 Magician的端口，取值范围：1~6。其中，port 1，port 2，port 4，port 5分别对应Magician的GP1，GP2，GP4，GP5。

- 返回：

  - 0： 光电传感器没有检测到物体。

  - 1： 光电传感器检测到物体。

- 
示例

```python
magician.get_infrared_sensor(port=1)

```

光电传感器与Magician的端口1连接，获取光电传感器的返回值。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置颜色传感器

- 
原型：

```python
magician.set_color_sensor(port, enable, version)

```

- 
描述：设置颜色传感器使能状态及版本。

- 
必选参数：

  - port：颜色传感器连接至 Magician的端口。取值：1~6。

  - enable：使能颜色传感器。True：使能；False：未使能。

  - version：颜色传感器版本。0：V1.0；1：V2.0。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_color_sensor(port=1, enable=True, version=0)

```

颜色传感器与Magician的端口1连接，控制颜色传感器上使能，并设置其版本为V1.0。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取颜色传感器读数

- 
原型：

```python
magician.get_color_sensor()

```

- 
描述：获取颜色传感器返回的像素值。

- 
必选参数：无

- 
返回：(r, g, b)

  - r： 红色，取值范围：0-255。

  - g： 绿色，取值范围：0-255。

  - b：蓝色，取值范围：0-255。

- 
示例

```python
magician.get_color_sensor()

```

获取颜色传感器返回的像素值。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 等待 n 秒

- 
原型：

```python
magician.wait(second)

```

- 
描述：设置等待时间。

- 
必选参数：  

  - second：等待时间，单位 s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.wait(second=10)

```

设置Magician等待10s。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 回零

- 
原型：

```python
magician.set_home()

```

- 
描述：Magician执行回零操作。

- 
必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_home()

```

Magician执行回零操作。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取当前位姿

- 
原型：

```python
magician.get_pose()

```

- 
描述：获取Magician当前位姿。

- 
必选参数：无

- 
返回：(x, y, z, r, jointAngle)

  - x：X 轴坐标。

  - y：Y 轴坐标。

  - z：Z 轴坐标。

  - r：R 轴坐标。

  - jointAngle：关节坐标列表 [关节 1,关节 2,关节 3,关节 4]。

- 
示例

```python
magician.get_pose()

```

获取Magician当前位姿。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取滑轨位姿

- 
原型：

```python
magician.get_posel()

```

- 
描述：获取滑轨位姿的坐标值。

- 
必选参数：无。

- 
返回：  

  - value：滑轨坐标值。

- 
示例

```python
magician.get_posel()

```

获取滑轨当前坐标值。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 清除报警

- 
原型：

```python
magician.clear_alarm()

```

- 
描述：清除报警。

- 必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.clear_alarm()

```

清除报警信息。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取机械臂速度比例

- 
原型：

```python
magician.get_arm_speed_ratio(mode)

```

- 
描述：获取Magician的速度比例。

- 
必选参数：

  - mode：运动模式，0：点动；1：点到点运动。

- 返回： 

  - ratio：对应运动模式的速度比例。

- 
示例

```python
magician.get_arm_speed_ratio(mode=1)

```

获取Magician的点到点运动模式对应的速度比例。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置丢步阈值

- 
原型：

```python
magician.set_lost_step_params(value)

```

- 
描述：设置丢步检测阈值，用于检测定位误差是否超过该阈值。如果超过该阈值，则说明电机丢步。

- 
必选参数： 

  - value：丢步检测阈值，数据类型：int。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_lost_step_params(value=10)

```

设置丢步检测阈值为10。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 执行检测丢步

- 
原型：

```python
magician.set_lost_step_cmd()

```

- 
描述：执行丢步检测。

- 
必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_lost_step_cmd()

```

执行丢步检测。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 检测丢步结果

- 
原型：

```python
magician.get_lost_step_result()

```

- 
描述：获取丢步检测的结果。

- 必选参数：无。

- 返回：

  - state：系统报警状态，数据类型：list。

- 
示例

```python
magician.get_lost_step_result()

```

获取丢步检测的结果。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置传送带速度参数并运动

- 
原型：

```python
magician.set_converyor(index,enable,speed)

```

- 
描述：设置传送带速度参数并控制传送带运动。

- 
必选参数：

  - index：电机序号，取值范围：0~1，也可以设置为字符，具体对应关系如下：

    - 0：magician.Stepper1。

    - 1：magician.Stepper2。 

  - enable：使能传送带。True：使能；False：未使能。

  - speed：电机控制速度，单位：毫米每秒。

- 
返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
magician.set_converyor(index=magician.Stepper1,enable=True,speed=250.0)

```

传送带以每秒250个脉冲的速度启动运行，其中，电机序号为magician.Stepper1。


                                
                                
                            
    

---

