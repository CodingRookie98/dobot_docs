# Dobot Magician Go Beta 视觉与复合动作指令

## 3.5 Dobot Magician Go Beta

---

## 进入停车位

- 原型：

```python
beta_go.into_park_space(garage_class)

```

- 描述：结合地图使用，Magician Go进入超市停车位或者进入仓库停车位。

- 必选参数：garage_class，停车位类型，0：仓库；1：超市。

- 返回：

  - True： 完成。

  - False： 未完成。

- 示例

将Magician Go放置在地图起点位置，启动巡线，Magician Go进入仓库停车位。

```python
go.set_odometer_data(x=0, y=0, yaw=0)               #复位(设置起点位置)
go.set_auto_trace(trace=1)                          #开启巡线
go.set_trace_speed(speed=20)                        #设置巡线速度
beta_go.stop_point(point=[250, 50], scope=20, err=2)#在目标点(250,50)停车
go.set_rotate(r=90, Vr=40)                           #旋转90°
beta_go.into_park_space(garage_class=0)              #进入仓库停车位

```

---

## 退出停车位

- 原型：

```python
beta_go.out_park_space(garage_class)

```

- 描述：结合地图使用，用于Magician Go退出超市停车位或者退出仓库停车位。

- 必选参数：garage_class，停车位类型，0：仓库；1：超市。

- 返回：

  - True： 完成。

  - False： 未完成。

- 示例

前提条件：Magician Go目前停在仓库停车位。

```python
beta_go.out_park_space(garage_class=0)

```

使Magician Go退出仓库停车位。

---

## 从车上抓取物品放置到地面

- 原型：

```python
beta_go.grab_obj_cartofloor(object_class)

```

- 描述：抓取Magician Go置物托盘上的物品(生鲜和/或快递)，放到地面的置物盒上。当摄像头视野内无物品时，进入下一条指令。

- 必选参数：object_class，物品类型，0：生鲜和快递；1：生鲜；2：快递。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
beta_go.grab_obj_cartofloor(object_class=0)

```

夹取Magician Go置物托盘上的生鲜和快递，放到地面的置物盒上。

---

## 从地面抓取物品放置到车上

- 原型：

```python
beta_go.grab_obj_floortocar(object_class)

```

- 描述：抓取地面置物盒上的物品(生鲜和/或快递)，放到Magician Go的置物托盘上。

- 必选参数：object_class，物品类型，0：生鲜和快递；1：生鲜；2：快递。

- 返回：

  - True： 指令完成。

  - False：指令未完成。

- 示例
```python
beta_go.grab_obj_floortocar(object_class=1)

```

抓取地面置物盒上的生鲜，放到Magician Go的置物托盘上。

---

## 判断是否到达目标点附近

- 原型：

```python
beta_go.stop_point(point,scope,err)

```

- 描述：Magician Go在运动过程中，实时判断是否进入以目标点为中心点的正方形区域内，其中，正方形的边长由scope确定。

  - 当Magician Go进入正方形区域内时，Magician Go继续前进，在距离目标点的前后距离小于err时，Magician Go停止运动。

  - 否则，Magician Go一直搜索以目标点为中心点的正方形区域(不会执行下一条指令)。

- 必选参数：

  - point：目标点的坐标 (X轴坐标，Y轴坐标)。

  - scope：正方形区域参数，数据类型：int，取值范围：15 cm ~ 30 cm ，推荐值：20 cm。

  - err：前后停车误差，数据类型：int。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
beta_go.stop_point(point=[100, 0], scope=20, err=2)

```

Magician Go在运动过程中，实时判断是否进入以目标点(100, 0)为中心点的正方形区域内，其中，正方形的边长为40cm（scope的2倍）；当Magician Go进入正方形区域内时，Magician Go继续前进，在距离目标点的前后距离小于2cm时，Magician Go停止运动。

---

## 将末端AI摄像头移动到车上检测点

- 原型：

```python
beta_go.set_ptp_car()

```

- 描述：将末端AI摄像头移动到Magician Go置物托盘上方的拍照位置（为末端AI摄像头对置物托盘上的物品进行目标检测做拍照准备）。

- 必选参数：无。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
beta_go.set_ptp_car()

```

将末端AI摄像头移动到Magician Go置物托盘上方的拍照位置。

---

## 将末端 AI 摄像头移动到地面检测点

- 原型：

```python
beta_go.set_ptp_floor()

```

- 描述：将末端AI摄像头移动到地面的置物盒上方的拍照位置（为末端AI摄像头对置物盒上的物品进行目标检测做拍照准备）。

- 必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
beta_go.set_ptp_floor()

```

将末端AI摄像头移动到地面的置物盒上方的拍照位置。

---

## 视觉目标坐标转化为机械臂坐标

- 原型：

```python
beta_go.imgxy_to_armxy(px,py,need_tranxy,suck_apriltag,apriltag_h)

```

- 描述：图像坐标转换为机械臂坐标。

- 必选参数：

  - px：图像 x 像素坐标。

  - py：图像 y 像素坐标。

  - need_tranxy：0：机械臂处于小车置物盒上方，1：机械臂处于地面上方。

  - suck_apriltag ：是否为贴有Apriltag码的物品，0：否；1，是。

  - apriltag_h：贴有Apriltag码的物品的高度。

- 返回：机械臂坐标系的X轴和Y轴坐标。

- 示例

```python
Mx，My = beta_go.imgxy_to_armxy(px=0, py=0, need_tranxy=0, suck_apriltag=0, apriltag_h=10)

```

将图像坐标(0,0)转换为机械臂坐标系的坐标。

---

## 创建二维码物体信息

- 原型：

```python
beta_go.creat_apriltag_obj(id,height)

```

- 描述：创建Apriltag码对应的物品信息。

- 必选参数：

  - id：Apriltag码的编号。

  - height：贴了Apriltag码的物品高度，单位：cm。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
beta_go.creat_apriltag_obj(0,10)

```

设置Apriltag码的ID为0，贴了该Apriltag码的物品高度是10 cm。

---

## 获取二维码物体高度

- 原型：

```python
beta_go.get_apriltag_obj_height(id)

```

- 描述：获取Apriltag码对应的物品的高度参数。其中，高度参数由beta_go.creat_apriltag_obj (id, height)进行创建。

- 必选参数：

  - id：Apriltag码的编号。

- 返回：

  - height：Apriltag码对应的物品的高度。

- 示例

```python
height = beta_go.get_apriltag_obj_height(id)
print(height)

```

获取Apriltag码对应的物品的高度参数。

---

## 获取二维码的机械臂Z轴坐标

- 原型：

```python
beta_go.get_apriltag_obj_z(id)

```

- 描述：获取放在置物托盘或置物盒上贴有Apriltag码的物品对应的机械臂Z轴坐标。

- 必选参数：

  - id：Apriltag码的编号。

- 返回：

  - z：机械臂Z轴坐标。

- 示例

```python
z = beta_go.get_apriltag_obj_z(id)
print(z)

```

获取放在置物托盘或置物盒上贴有Apriltag码的物品对应的机械臂Z轴坐标。

---

## 设置末端AI摄像头检测模型

- 原型：

```python
beta_go.set_arm_camera_model(index)

```

- 描述：设置末端AI摄像头检测模型。

- 必选参数：index，检测模型。1：积木识别模型；2：二维码识别模型；3：生鲜快递模型。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
beta_go.set_arm_camera_model(index=1)

```

设置末端AI摄像头检测模型。

---

## 设置底盘AI摄像头检测模型

- 原型：

```python
beta_go.set_car_camera_model(index)

```

- 描述：设置底盘AI摄像头检测模型。

- 必选参数：index，检测模型。0：路标识别模型。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
beta_go.set_car_camera_model(index)

```

设置底盘AI摄像头检测模型。

---

## 获取末端AI摄像头检测模型

- 原型：

```python
beta_go.get_arm_camera_model()

```

- 描述：获取末端AI摄像头检测模型。

- 必选参数：无

- 返回：index，检测模型。0：路标识别模型；1：积木识别模型；2：二维码识别模型；3：生鲜快递模型。

- 示例

```python
beta_go.get_arm_camera_model()

```

获取末端AI摄像头检测模型。

---

## 获取底盘AI摄像头检测模型

- 原型：

```python
beta_go.get_car_camera_model()

```

- 描述：获取底盘AI摄像头检测模型。

- 必选参数：无

- 返回：index，检测模型。0：路标识别模型；1：积木识别模型；2：二维码识别模型；3：生鲜快递模型。

- 示例

```python
beta_go.get_car_camera_model()

```

获取底盘AI摄像头检测模型。

---

## 判断末端 AI 摄像头是否检测到目标

- 原型：

```python
beta_go.arm_camera_is_detected(obj_name)

```

- 描述：用于判断末端AI摄像头是否检测到obj_name对应的目标。

- 必选参数：obj_name，目标名称，数据类型：str。

| obj_name | obj_name对应的目标 |
| --- | --- |
| red | 红 |
| yellow | 黄 |
| blue | 蓝 |
| green | 绿 |
| orange | 橙子 |
| cabbage | 白菜 |
| water | 矿泉水 |
| dexp | 国内快递 |
| iexp | 国际快递 |
| cexp | 同城快递 |

- 返回：

  - True： 检测到obj_name对应的目标。

  - False： 未检测到obj_name对应的目标。

- 示例
```python
beta_go.arm_camera_is_detected(obj_name="red")

```

判断末端 AI 摄像头是否检测到红色物品。

---

## 判断底盘 AI 摄像头是否检测到目标

- 原型：

```python
beta_go.car_camera_is_detected(sign_name)

```

- 描述：用于判断底盘AI摄像头是否检测到obj_name对应的指示牌。

- 必选参数：obj_name，指示牌目标名称，数据类型：str。

| obj_name | obj_name对应的目标 |
| --- | --- |
| lors | 左转或者直行指示牌 |
| l | 左转指示牌 |
| p | 泊车指示牌 |
| apt | 住宅指示牌 |
| rors | 右转或者直行指示牌 |
| r | 右转指示牌 |
| stop | 停止指示牌 |
| spm | 超市指示牌 |
| t | T 字路口指示牌 |
| u | U 弯（掉头）指示牌 |
| wh | 仓库指示牌 |
| z | 斑马线 |

- 返回：

  - True： 检测到obj_name对应的指示牌。

  - False： 未检测到obj_name对应的指示牌。

- 示例
```python
beta_go.car_camera_is_detected(sign_name="r")

```

判断底盘 AI 摄像头是否检测到右转指示牌。

---
