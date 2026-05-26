# Dobot Magic Box 与基础外设工具指令

## 3.7 Dobot Magic Box

---

## 设置扩展电机速度参数

- 原型：

```python
magicbox.set_emotor(index, enable, speed)

```

- 描述：设置扩展电机的使能状态和速度参数。

- 必选参数：

  - index：电机编号。0：Stepper1；1：Stepper2。

  - enable：使能电机。True：使能；False：未使能。

  - speed：电机速度。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_emotor(index=1, enable=True, speed=50)

```

设置编号为1的扩展电机为上使能状态，并设置其速度为50。

---

## 设置颜色传感器

- 原型：

```python
magicbox.set_color_sensor(port, enable, version)

```

- 描述：设置颜色传感器使能状态及版本。

- 必选参数：

  - port：颜色传感器连接至 Dobot Magic Box 的端口，取值范围：1~6。

  - enable：使能颜色传感器，True：使能；False：未使能。

  - version：颜色传感器版本，0：V1.0；1：V2.0。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_color_sensor(port=1, enable=True, version=1)

```

颜色传感器与Dobot Magic Box 的端口1连接，控制颜色传感器上使能，并设置其版本为V1.0。

---

## 获取颜色传感器读数

- 原型：

```python
magicbox.get_color_sensor()

```

- 描述：获取颜色传感器返回的像素值。

- 必选参数：无

- 返回：(r, g, b)

  - r： 红色，取值范围：0-255。

  - g： 绿色，取值范围：0-255。

  - b：蓝色，取值范围：0-255。

- 示例

```python
magicbox.get_color_sensor()

```

获取颜色传感器返回的像素值。

---

## 设置光电传感器

- 原型：

```python
magicbox.set_infrared_sensor(port, enable, version)

```

- 描述：设置光电传感器使能状态及版本。

- 必选参数：

  - port：光电传感器连接至 Dobot Magic Box 的端口，取值范围：1~6。

  - enable：使能光电传感器。True：使能；False：未使能。

  - version：光电传感器版本。0：V1.0；1：V2.0。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_infrared_sensor(port=1, enable=True, version=1)

```

光电传感器与Dobot Magic Box 的端口1连接，控制光电传感器上使能，并设置其版本为V2.0。

---

## 获取光电传感器读数

- 原型：

```python
magicbox.get_infrared_sensor(port)

```

- 描述：获取光电传感器的返回值。

- 必选参数：

  - port：光电传感器连接至 Dobot Magic Box 的端口，取值范围：1~6。

- 返回：

  - 0： 光电传感器没有检测到物体。

  - 1： 光电传感器检测到物体。

- 示例

```python
magicbox.get_infrared_sensor(port=1)

```

光电传感器与Dobot Magic Box 的端口1连接，获取光电传感器的返回值。

---

## 设置滑轨开关及版本

- 原型：

```python
magicbox.set_device_withl(enable, version)

```

- 描述：设置滑轨的开关状态以及版本。

- 必选参数：

  - enable：使能滑轨，True：使能；False：未使能。

  - version：滑轨版本号。0：V1 版本；1：V2 版本。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_device_withl(enable=True, version=0)

```

滑轨上使能，并设置滑轨版本为V1 版本。

---

## 滑轨点到点运动速度比例

- 原型：

```python
magicbox.set_lspeed_ratio(set_type, set_value)

```

- 描述：设置滑轨不同模式下的运动速度比率。

- 必选参数：

  - set_type：0：点动模式，1：点到点运动模式。

  - set_value：速度范围：1-100。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_lspeed_ratio(set_type=1, set_value=100)

```

设置滑轨在点到点运动模式下的运动速度比率为100%。

---

## 滑轨点到点运动

- 原型：

```python
magicbox.set_ptpwithl_cmd(set_l)

```

- 描述：运动到设定的滑轨位姿。

-
参数：

  - set_l：滑轨坐标值。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_ptpwithl_cmd(set_l=100)

```

运动到设定的滑轨坐标为100的位置。

---

## 获取滑轨位姿

- 原型：

```python
magicbox.get_posel()

```

- 描述：获取滑轨位姿。

- 必选参数：无

- 返回：

  - value：滑轨坐标值。

- 示例

```python
magicbox.get_posel()

```

获取滑轨当前坐标值。

---

## 设置传送带速度参数并运动

- 原型：

```python
magicbox.set_converyor(index,enable,speed)

```

- 描述：设置传送带速度参数并控制传送带运动。

- 必选参数：

  - index：电机序号，取值范围：0~1，也可以设置为字符，具体对应关系如下：

    - 0：magicbox.STP1。

    - 1：magicbox.STP2。

  - enable：使能传送带。True：使能；False：未使能。

  - speed：电机控制速度，单位：脉冲每秒。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_converyor(index=magicbox.STP1,enable=True,speed=250.0)

```

传送带以每秒250个脉冲的速度启动运行，其中，电机序号为magicbox.STP1。

---

## 设置端口模式

- 原型：

```python
magicbox.set_port(port, io_func)

```

- 描述：设置端口模式。

- 必选参数：

  - port：EIO 地址，范围：1~26。

  - io_func：端口模式，取值范围 0-6，也可以设置为字符，具体对应关系如下：

    - 0：magicbox.DUMMY，不配置功能；

    - 1：magicbox.DO，IO 输出；

    - 2：magicbox.PWM，PWM 输出；

    - 3：magicbox.DI，IO 输入；

    - 4：magicbox.ADC，AD 输入；

    - 5：magicbox.DIPU，上拉输入；

    - 6：magicbox.DIPD，下拉输入。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_port(port=1, io_func=magicbox.DO)

```

设置EIO1端口的模式为IO 输出。

---

## 输出数字信号电平

- 原型：

```python
magicbox.set_io(port,level)

```

- 描述：设置数字端口输出的电平。

- 必选参数：

  - port：EIO 地址，范围：1-26。

  - level：输出电平，0：低电平，1：高电平。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_io(port=1,level=1)

```

设置EIO1端口为高电平输出。

---

## 输出PWM频率及占空比

- 原型：

```python
magicbox.set_pwm(port, frequency, duty_cycle)

```

- 描述：设置 PWM 输出端口的频率及占空比。

- 必选参数：

  - port：EIO 地址，范围：1-26。

  - frequency：PWM 频率，取值范围：16Hz-10KHz。

  - duty_cycle：占空比，取值范围：0-100。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例

```python
magicbox.set_pwm(port=1, frequency=16.2, duty_cycle=30.0)

```

设置EIO1端口的PWM 频率为16.2Hz，其占空比为30%。

---

## 获取数字信号输出

- 原型：

```python
magicbox.get_do(port)

```

- 描述：获取EIO接口输出的数字信号。

- 必选参数：

  - port：EIO 地址，范围：1~26。

- 返回：

  - port：EIO 地址。

  - level：输出电平，0：低电平，1：高电平。

- 示例

```python
magicbox.get_do(port=1)

```

获取EIO1端口输出的数字信号(高电平或低电平)。

---

## 获取数字信号输入

- 原型：

```python
magicbox.get_di(port)

```

- 描述：获取EIO接口输入的数字信号。

- 必选参数：

  - port：EIO 地址，范围：1~26。

- 返回：

  - port：EIO 地址。

  - level：输入电平，0：低电平，1：高电平。

- 示例

```python
magicbox.get_di(port=1)

```

获取EIO1端口输入的数字信号(高电平或低电平)。

---

## 获取模拟信号

- 原型：

```python
magicbox.get_ad(port)

```

- 描述：获取EIO接口的模拟信号。

- 必选参数：

  - port：EIO 地址，范围：1~26。

- 返回：

  - port：EIO 地址。

  - level：模拟信号。

- 示例

```python
magicbox.get_ad(port=1)

```

获取EIO1接口的模拟信号。

---

## 获取滑轨速度比例

- 原型：

```python
magicbox.get_rail_speed_ratio()

```

- 描述：获取滑轨的速度比例。

- 必选参数：无

- 返回：

  - vel：滑轨速度比例，范围：0~100。

- 示例

```python
magicbox.get_rail_speed_ratio()

```

获取滑轨的速度比例。

---

## 获取 pixy 摄像头颜色标识物体参数

- 原型：

```python
magicbox.get_pixy_camera_obj(port,color,coordinate)

```

- 描述：获取 pixy 摄像头显示的颜色标识物体的参数。

- 必选参数：

  - port：端口号，范围：1-6。

  - color：颜色标识，范围：1-7。

  - coordinate：坐标轴，范围：1~4 (1 代表 x, 2 代表 y, 3 代表 l, 4 代表 z)。

- 返回：

  - color：颜色标识。

  - coordinate：对应坐标参数。

- 示例

```python
magicbox.get_pixy_camera_obj(port=1,color=1,coordinate=1)

```

获取端口1连接的 pixy 摄像头，其显示的颜色标识对应的坐标参数。

---

## 判断pixy摄像头是否检测到颜色标识物体

- 原型：

```python
magicbox.get_pixy_camera_is_detected(port, color)

```

- 描述：判断pixy摄像头是否检测到颜色标识物体。

- 必选参数：

  - port：端口号，范围：1-6。

  - color：颜色标识，范围：1-7。

- 返回：

  - True：True 检测到颜色标识物体。

  - False：未检测到颜色标识物体。

- 示例

```python
magicbox.get_pixy_camera_is_detected(port=1, color=1)

```

判断 pixy 摄像头是否检测到颜色标识物体。

---

## 设置蓝牙群组和设备 id

- 原型：

```python
magicbox.set_bt_mesh(group, id)

```

- 描述：设置蓝牙群组的设备 id。

- 必选参数：

  - group：蓝牙群组名， 取值范围：长度 6 个字节，每个字节都为数字0-9。

  - id：群组ID，取值范围：0-255。

- 返回：

  - True：设置成功。

  - False：设置失败。

- 示例

```python
magicbox.set_bt_mesh(group="123456", id=1)

```

设置蓝牙群组的群组名为"123456"，设备 id为1。

---

## 发送蓝牙信息

- 原型：

```python
magicbox.set_bt_send(to_id, text)

```

- 描述：发送蓝牙信息。

- 必选参数：

  - to_id：设备 id，范围：0-255。

  - text：发送的消息，数据类型：str。

- 返回：

  - True：设置成功。

  - False：设置失败。

- 示例

```python
magicbox.set_bt_send(to_id=1, text="hello")

```

向设备 id为1的蓝牙群组发送"hello"。

---

## 获取设备的蓝牙返回信息

- 原型：

```python
magicbox.get_bt_receive(from_id)

```

- 描述：获取蓝牙群组的返回信息。

- 必选参数：

  - from_id：设备 id，范围：0-255。

- 返回：

  - text：接收的消息。

- 示例

```python
magicbox.get_bt_receive(from_id=1)

```

获取设备 id为1的蓝牙群组的返回信息。

---

## 判断是否收到设备的蓝牙返回信息

- 原型：

```python
magicbox.get_bt_is_received(from_id, text)

```

- 描述：判断是否收到设备的蓝牙返回信息。该 API只判断一次当前是否接收到蓝牙的返回信息。

- 必选参数：

  - from_id：设备 id，范围：0-255。

  - text：接收的消息。

- 返回：

  - True：接收成功。

  - False：接收失败。

- 示例

```python
magicbox.get_bt_is_received(from_id=1, text="hello")

```

判断设备 id为1的蓝牙群组是否收到"hello"这个信息。

---

## 当收到设备发送的蓝牙信息

- 原型：

```python
magicbox.get_bt_until_received(from_id, text)

```

- 描述：判断是否收到设备的蓝牙返回信息。该 API在没有收到蓝牙信息的时候会一直等待，直到接收到信息才会结束。

- 必选参数：

  - from_id：设备 id，范围：0-255。

  - text：接收的消息。

- 返回：

  - True：接收成功信息。

  - False：未收到信息时一直等待。

- 示例

```python
magicbox.get_bt_until_received(from_id=1, text="hello")

```

判断设备 id为1的蓝牙群组是否收到"hello"这个信息，如果未收到信息时，则一直等待。

---

## 清除蓝牙信息缓存

- 原型：

```python
magicbox.clean_bt_cache()

```

- 描述：清除蓝牙信息缓存。

- 必选参数：无

- 返回：

  - True：缓存清除成功。

  - False：缓存清除失败。

- 示例

```python
magicbox.clean_bt_cache()

```

清除蓝牙信息缓存。

---

## 设置舵机角度

- 原型：

```python
magicbox.set_servo_angle(port, angle)

```

- 描述：设置舵机角度。

- 必选参数：

  - port：控制盒端口。 数据类型：int，取值范围：1 ~ 6。

  - angle:角度。数据类型：float，取值范围：-180 ~ 180。

- 返回：

  - True：设置成功。

  - False：未设置成功。

- 示例

```python
magicbox.set_servo_angle(port=1, angle=90)

```

设置与控制盒port1连接的舵机角度为90°。

---
