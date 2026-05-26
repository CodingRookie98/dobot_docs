# Dobot Magician Go 基础小车控制指令


                            

    
    
                                
                                
                                
## 3.4 Dobot Magician Go


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置运行模式

- 
原型：

```python
go.set_running_mode(mode)

```

- 
描述：开启或关闭安全模式。

- 
必选参数：mode，运行模式。0：关闭安全模式；1：开启安全模式。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_running_mode(mode=1)

```

  开启安全模式。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置里程计数据

- 
原型：

```python
go.set_odometer_data(x,y,yaw)

```

- 
描述：设置Magician Go的里程计数据，即Magician Go的坐标及航向角。

- 
必选参数：

  - x：X轴坐标，数据类型：float，单位：cm。

  - y：Y轴坐标，数据类型：float，单位：cm。

  - yaw：Magician Go的航向角，数据类型：float，单位：° (度)。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_odometer_data(x=0,y=0,yaw=0)

```

设置Magician Go的当前位置为坐标原点，即复位操作。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置平移方向和速度参数

- 
原型：

```python
go.set_move_speed_direct(direction,speed)

```

- 
描述：设置Magician Go的平移方向和速度参数。

- 
必选参数：

  - 
direction：Magician Go的平移方向，数据类型：float，取值范围：-180° ~ 180°。

其中，Magician Go的当前位置为0 °，逆时针方向角度为正值，顺时针方向角度为负值。

  - 
speed：Magician Go的平移速度，数据类型：float，取值范围：0 ~ 100 cm/s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_move_speed_direct(direction=0,speed=20)

```

设置Magician Go的平移方向为0° (向前)，移动速度为20 cm/s。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置移动速度参数

- 
原型：

```python
go.set_move_speed(x,y,r)

```

- 描述：设置Magician Go的移动速度。

- 必选参数：

  - x：Magician Go的X轴移动速度，数据类型：float，取值范围：-100 cm/s ~ 100 cm/s。
其中，当x的取值为正数时，表示沿X轴正方向移动；当x的取值为负数时，表示沿X轴负方向移动。

  - y：Magician Go的Y轴移动速度，数据类型：float，取值范围：-100 cm/s ~ 100 cm/s。
其中，当y的取值为正数时，表示沿Y轴正方向移动；当y的取值为负数时，表示沿Y轴负方向移动，。

  - r ：Magician Go的旋转速度，数据类型：float，取值范围：-100 °/s ~ 100 °/s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_move_speed(x=10,y=0,r=0)

```

设置Magician Go沿X轴正方向移动速度为10 cm/s。Magician Go的X轴和Y轴方向如下图所示。



---


                            

    
    
                                
                                
                                
## 设置旋转角度和旋转速度参数

- 
原型：

```python
go.set_rotate(r,Vr)

```

- 
描述：设置Magician Go的旋转偏移角度和旋转速度。

- 
必选参数：

  - r：Magician Go的旋转偏移角度，数据类型：float，单位：° (度)。
其中，Magician Go的当前位置为0 °，角度为正值时，Magician Go逆时针方向旋转；角度为负值，Magician Go顺时针方向旋转。

  - Vr：Magician Go的旋转速度，数据类型：float，单位：° /s，取值范围: 0 ~ 100 ° /s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_rotate(r=20,Vr=10)

```

设置Magician Go的偏移角度为20°，旋转速度为10 ° /s。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置X轴Y轴移动距离及移动速度参数

- 
原型：

```python
go.set_move_dist(x,y,Vx,Vy)

```

- 
描述：设置Magician Go沿X轴的偏移距离和移动速度，以及沿Y轴的偏移距离和移动速度。Magician Go的X轴和Y轴方向如下图所示。



---


                            

    
    
                                
                                
                                
## 移动到目标点

- 
原型：

```python
go.set_move_pos(x,y,s)

```

- 
描述：Magician Go以设置的速度移动到目标点。

- 
必选参数：

  - x：目标点的X轴坐标，数据类型：float，单位：cm。

  - y：目标点的Y轴坐标，数据类型：float，单位：cm。

  - s：Magician Go的移动速度，数据类型：float，取值范围：0 ~ 100 cm/s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_move_pos(x=100,y=100,s=20)

```

Magician Go以20 cm/s的速度移动到目标点(100 cm,100 cm)。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 以半径方式走圆弧轨迹

- 
原型：

```python
go.set_arc_rad(velocity,radius,angle,mode)

```

- 描述：由Magician Go当前位置和半径确定圆形轨道，Magician Go从当前位置出发，沿着圆形轨道移动到目标角度。

- 
必选参数：

  - velocity：Magician Go的圆弧运动速度，数据类型：float，单位：°/s，取值范围：0 ~ 100 °/s。

  - radius：圆弧运动半径，数据类型：float，单位：cm。

  - angle：目标圆弧角度，数据类型：float，单位：° (度)。

  - 
mode：圆弧运动的行走模式。

    - 
1：切向运动模式，如下图所示。



---


                            

    
    
                                
                                
                                
## 以圆心方式走圆弧轨迹

- 
原型：

```python
go.set_arc_cent(velocity,x, y,angle,mode)

```

- 描述：将Magician Go的车身中心作为原点，由Magician Go当前位置和圆心坐标确定圆形轨道，Magician Go从当前位置出发，沿着圆形轨道移动到目标角度。

- 
必选参数：

  - velocity：Magician Go的圆弧运动速度，数据类型：float，单位：°/s，取值范围：0 ~ 100 °/s。

  - x：圆心的X轴坐标，数据类型：float，单位：cm。

  - y：圆心的Y轴坐标，数据类型：float，单位：cm。

  - angle：目标角度，数据类型：float，单位：° (度)。

  - 
mode：圆弧运动的行走模式。

    - 
1：车头方向不变模式，如下图所示。



---


                            

    
    
                                
                                
                                
## 设置角度闭环

- 
原型：

```python
go.set_coord_closed_loop(isEnable,angle)

```

- 
描述：开启或关闭角度闭环功能，其中，角度闭环是指Magician Go在运动过程中保持固定的航向角。

- 
必选参数：

  - isEnable：角度闭环状态。0：关闭；1：开启。

  - angle：航向角，数据类型：float，取值范围：-180 °~ 180°。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_coord_closed_loop(isEnable=1,angle=90)

```

开启角度闭环功能，航向角为90°。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置编程灯状态

- 
原型：

```python
go.set_rgb_light(number,effect,r,g,b,cycle,counts)

```

- 
描述：设置编程灯状态。

- 
必选参数：

  - number：编程灯编号或对应值。

    - “LED_1”或1：左尾编程灯；

    - “LED_2”或2：右尾编程灯；

    - “LED_3”或3：右前编程灯；

    - “LED_4”或4 ：左前编程灯；

    - “LED_ALL”或5：全部编程灯。

  - effect：编程灯状态。

    - 0：常亮模式；

    - 1：定时熄灭；

    - 2：呼吸模式；

    - 3：闪烁模式；

    - 4：彩虹呼吸渐变模式；

    - 5：流水环绕；

    - 0xff：与状态指示灯的状态一致。

  - r：红色亮度值，数据类型：int，取值范围：0 ~ 255。

  - g：绿色亮度值，数据类型：int，取值范围：0 ~ 255。

  - b：蓝色亮度值，数据类型：int，取值范围：0 ~ 255。

  - cycle：周期，数据类型：float，单位： s。

  - counts：仅在闪烁模式有效，表示闪烁次数：-1：无限次；1：1 次，2：2 次，以此类推。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_rgb_light(number="LED_1", effect=1,r=255,g=0,b=0,cycle=2,counts=2)

```

设置左尾编程灯为定时熄灭模式，该编程灯的颜色为红色，亮起2s后熄灭。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置蜂鸣器音效

- 
原型：

```python
go.set_buzzer_sound(index,tone,beat)

```

- 
描述：设置蜂鸣器音效。

- 
必选参数：

  - index：蜂鸣器的音效编号。

    - 0：关闭音效

    - 1：鸣叫

    - 2：定时关闭音效

    - 3：滴

    - 4：滴滴滴

    - 5：滴~滴 滴

    - 6：滴滴滴滴滴 12345 (1234567 代表唱名 do、re、mi、fa、so、la、xi)

  - tone：当index = 1或2时，tone参数有效，表示钢琴键音调。数据类型：int，取值范围：0 ~ 84 (分别代  表不同的钢琴键)，推荐设置40 ~ 60。            

  - beat：当index = 2时，beat参数有效，表示节拍数，数据类型：int，单位：s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_buzzer_sound(index=2, tone=50, beat=2)

```

蜂鸣器以第50钢琴键音调鸣叫2s后停止。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取超声波数据

- 
原型：

```python
go.get_ultrasonic_data()

```

- 
描述：超声波传感器对检测范围内的障碍物进行检测，检测范围：2cm ~ 40 cm，该指令用于获取超声波传感器的检测数据。

- 
必选参数：无

- 
返回：{front,back,left,right}

  - 
front： 正前方超声波传感器检测到障碍物的距离，单位 cm。

  - 
back： 正后方超声波传感器检测到障碍物的距离，单位 cm。

  - 
left：左边超声波传感器检测到障碍物的距离，单位 cm。

  - 
right：右边超声波传感器检测到障碍物的距离，单位 cm。

其中，返回值为0时，表示超声波传感器故障；返回值为40时，表示未检测到障碍物；返回值为255时，表示超声波传感器未打开。

- 
示例

```python
result = go.get_ultrasonic_data( )
print (result)

```

获取超声波传感器的检测数据。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取里程计数据

- 
原型：

```python
go.get_odometer_data()

```

- 
描述：获取里程计数据，即获取Magician Go当前位置的坐标和航向角。

- 
必选参数：无

- 返回：{x, y, yaw}

  - x：X轴坐标，数据类型：float，单位：cm。

  - y：Y轴坐标，数据类型：float，单位：cm。

  - yaw：Magician Go的航向角，数据类型：float，单位：° (度)。

- 
示例

```python
result = go.get_odometer_data( )  
print(result)

```

 获取Magician Go当前位置的坐标和航向角。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取电池电压

- 
原型：

```python
go.get_power_voltage()

```

- 
描述：获取Magician Go的电池电压和电池电量。

- 
必选参数：无

- 
返回：{powerVoltage, powerPercentage}

  - powerVoltage：电池电压，数据类型：float，单位：V。

  - powerPercentage：剩余电池电量的比例，数据类型：float，范围：0 ~ 1。

- 
示例

```python
result = go.get_power_voltage( )  
print(result)

```

获取Magician Go的电池电压和剩余电池电量的比例。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取IMU角度数据

- 
原型：

```python
go.get_imu_angle()

```

- 
描述：获取Magician Go的IMU角度数据。

- 
必选参数：无

- 返回：{yaw, roll, pitch}

  - yaw：IMU航向角，数据类型：float，单位：° (度)。

  - roll：IMU横滚角，数据类型：float，单位：° (度)。

  - pitch：IMU俯仰角，数据类型：float，单位：° (度)。

- 
示例

```python
result = go.get_imu_angle()  
print(result)

```

获取Magician Go的IMU的角度数据。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 自动巡线

- 
原型：

```python
go.set_auto_trace(trace)

```

- 描述：开启或关闭自动巡线功能。

  - 开启自动巡线功能时，系统默认巡线速度为20 cm/s，pid为(0.5，0，0.5)，Magician Go开始巡线；关闭自动巡线功能时，系统默认巡线速度为0，巡线停止。

  - 开启巡线功能后，其他运动控制指令不能使用。

  - 如果已打开安全开关，则遇到障碍物时仍会自动停止。

- 必选参数：

  - trace：自动巡线状态。0：关闭自动巡线功能；1：开启自动巡线功能。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_auto_trace(trace=1)

```

Magician Go开启自动巡线功能。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置巡线速度参数

- 
原型：

```python
go.set_trace_speed(speed)

```

- 
描述：设置巡线速度。

- 
必选参数：

  - speed：巡线速度。数据类型：float，取值范围：0 ~ 30 cm/s。速度大于 20 cm/s时，需要设置pid参数；速度小于5 cm/s时，Magician Go运动不明显。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_auto_trace(trace=1)  
go.set_trace_speed(speed=20)

```

开启自动巡线功能，并设置巡线速度为20 cm/s。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 设置巡线PID

- 
原型：

```python
go.set_trace_pid(p,i,d)

```

- 描述：与设置巡线速度一起使用，有的时候更新巡线速度之后，发现小车巡线效果不好，可以调节PID这些参数来改善Magician Go的巡线效果。

- 必选参数：

  - p：巡线 p (比例)值。数据类型：float，推荐值：0.5。

  - i：巡线 i (积分)值。数据类型：float，推荐值：0。

  - d：巡线 d(微分) 值。数据类型：float，推荐值：0.5。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 
示例

```python
go.set_trace_pid(p=0.5,i=0,d=0.5)

```

设置巡线 PID参数。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取巡线角度数据

- 
原型：

```python
go.get_trace_angle()

```

- 描述：Magician Go在巡线时，用于获取巡线的角度。其中，角度为：Magician Go车头方向与道路中心线的夹角。

- 必选参数：无

- 返回：    

  - angle： 角度。

- 
示例

```python
angle = go.get_trace_angle()
print(angle)

```

获取Magician Go巡线的角度。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取末端AI摄像头目标检测数据

- 
原型：

```python
go.get_arm_camera_obj()

```

- 
描述：获取末端 AI 摄像头所检测到的目标物品对应的检测数据 。

- 
必选参数：无

- 返回：{count, dl_obj[count]}

  - count： 目标物品的总数量。

  - dl_obj [i]={x，y，w，h，ID}：目标物品在视觉坐标系的参数。

    - x：图像识别检测框中心点的X轴坐标

    - y：图像识别检测框中心点的Y轴坐标

    - w：图像识别检测框的宽度

    - h：图像识别检测框的高度

    - ID：物品的类别

当末端 AI 摄像头的检查类型为积木检测时，ID对应的类别如下： 

| ID | 类别名字（中文） | 类别名字（英文） |
| --- | --- | --- |
| 0 | 红 | red |
| 1 | 黄 | yellow |
| 2 | 蓝 | blue |
| 3 | 绿 | green |

当末端 AI 摄像头的检查类型为快递生鲜检测时，ID对应的类别如下：

| ID | 类别名字（中文） | 类别名字（英文） |
| --- | --- | --- |
| 0 | 橙子 | Orange |
| 1 | 白菜 | Cabbage |
| 2 | 矿泉水 | Water Bottle |
| 3 | 国内快递 | Domestic Express |
| 4 | 国际快递 | International Express |
| 5 | 同城快递 | City Express |

- 
示例

```python
datalist = go.get_arm_camera_obj()                      # 得到末端摄像头检测的信息
if datalist["count"]:                                   # 如果控制盒上存在积木块
   grab_ind = randint(0,int(datalist["count"]-1))          #随机选取一个积木块
   grab_obj = datalist["dl_obj"][grab_ind]                 # 得到积木块的信息
   x_c = grab_obj["x"]+grab_obj["w"]/2                     # 计算积木块中心点坐标
   y_c = grab_obj["y"]+grab_obj["h"]/2

```

  获取末端 AI 摄像所检测到的目标物品对应的检测数据。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取底盘AI摄像头目标检测数据

- 
原型：

```python
go.get_car_camera_obj()

```

- 
描述：获取底盘AI摄像头所检测到的目标物品对应的检测数据 。

- 
必选参数：无

- 
返回：{count, dl_obj[count]}

  - count： 目标物品的总数量。

  - dl_obj [i]={x，y，w，h，ID}：目标物品在视觉坐标系的参数。

    - x：图像识别检测框中心点的X轴坐标

    - y：图像识别检测框中心点的Y轴坐标

    - w：图像识别检测框的宽度

    - h：图像识别检测框的高度

    - ID：物品的类别

| ID | 路标名（中文） | 路标名（英文） |
| --- | --- | --- |
| 0 | 左转或者直行指示牌 | Turn Left or Go Straight Sign |
| 1 | 左转指示牌 | Turn Left Sign |
| 2 | 泊车指示牌 | Parking Sign |
| 3 | 住宅指示牌 | Apartment Sign |
| 4 | 右转或者直行指示牌 | Turn Right or Go Straight Sign |
| 5 | 右转指示牌 | Turn Right Sign |
| 6 | 停止指示牌 | STOP Sign |
| 7 | 超市指示牌 | Supermarket Sign |
| 8 | T 字路口指示牌 | T-junction Sign |
| 9 | U 弯（掉头）指示牌 | U turn Sign |
| 10 | 仓库指示牌 | Intelligent Warehouse Sign |
| 11 | 斑马线 | zebra crossing |

- 
示例

```python
go.get_car_camera_obj()

```

获取底盘AI摄像头所检测到的目标物品对应的检测数据。


                                
                                
                            
    

---


                            

    
    
                                
                                
                                
## 获取末端AI摄像头二维码检测数据

- 
原型：

```python
go.get_arm_camera_tag()

```

- 
描述：末端 AI 摄像检测到贴有 Apriltag 码的物品时，获取 Apriltag 码的参数。

- 
必选参数：无

- 返回：{count, dl_obj[count]}

  - count： 目标物品的总数量。

  - dl_obj [i]={x，y，w，h，ID}：目标物品在视觉坐标系的参数。

    - x：图像识别检测框中心点的X轴坐标

    - y：图像识别检测框中心点的Y轴坐标

    - w：图像识别检测框的宽度

    - h：图像识别检测框的高度

    - ID： Apriltag 码的编号

- 
示例

```python
res = go.get_arm_camera_tag()
print(res)

```

获取末端 AI 摄像所检测到的 Apriltag 码对应的检测数据。


                                
                                
                            
    

---

