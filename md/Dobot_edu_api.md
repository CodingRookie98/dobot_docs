# DobotEDU Python SDK 接口文档 (v2.2.2)

本库提供了对 `Magician Go` 全向小车、`Magician Lite` 机械臂以及多种 AI 视觉服务的控制接口。

## 1. 快速入门

### 初始化
```python
from DobotEDU import *

# 默认已初始化全局对象：
# go: Magician Go 小车控制
# m_lite: Magician Lite 机械臂控制
# beta_go: 视觉与高层逻辑控制
# util: 基础外设工具 (摄像头/麦克风)
# ocr, face, speech, nlp, tmt, robot, ai(pyimageom): AI 及辅助视觉服务
```

---

## 2. Magician Go 控制 (`go`)

`go` 对象用于控制全向小车的运动、传感器及灯光。

### 运动控制 (Movement)
- `set_move_speed_direct(direction, speed)`: 设置直接方向的相对移动速度。
- `set_move_speed(x, y, r)`: 设置全向移动速度。
- `set_rotate(r, Vr)`: 相对当前方向旋转 `r` 度，速度为 `Vr`。
- `set_move_dist(x, y, Vx, Vy)`: 移动指定距离 `(x, y)`，速度为 `(Vx, Vy)`。
- `set_move_pos(x, y, s)`: 移动到绝对坐标 `(x, y)`，线速度为 `s`。

### 巡线控制 (Line Tracking)
- `set_auto_trace(trace)`: 开启 (`1`) 或关闭 (`0`) 自动巡线。
- `set_trace_speed(speed)`: 设置巡线速度。
- `set_trace_pid(p, i, d)`: 设置巡线 PID 参数。

### 传感器数据 (Sensors)
- `get_power_voltage()`: 获取小车电池电量，返回 `powerVoltage` 和 `powerPercentage`。
- `get_ultrasonic_data()`: 获取超声波避障数据，返回包含 `front`, `back`, `left`, `right` 距离的字典。
- `get_odometer_data()`: 获取里程计数据，返回 `x`, `y`, `yaw`。
- `set_odometer_data(x, y, yaw)`: 改写/校准里程计数据。
- `get_imu_angle()`: 获取 6 轴 IMU 姿态角 (`yaw`, `roll`, `pitch`)。
- `get_imu_speed()`: 获取 6 轴 IMU 加速度与角速度 (`ax`, `ay`, `az`, `gx`, `gy`, `gz`)。

### 交互控制 (Interaction)
- `set_rgb_light(number, effect, r, g, b, cycle, counts)`: 设置板载 RGB 灯效。
  - `number`: `"LED_1"` 到 `"LED_4"` 或 `"LED_ALL"`。
- `set_buzzer_sound(index, tone, beat)`: 控制蜂鸣器发声。

---

## 3. Magician Lite 机械臂控制 (`m_lite`)

`m_lite` 对象用于控制机械臂的精确姿态。

### 点位运动 (PTP)
- `set_ptpcmd(ptp_mode, x, y, z, r, is_queued=True, is_wait=True)`: 执行 PTP 运动目标。
  - `ptp_mode`: `0` (JUMP), `1` (MOVJ), `2` (MOVL)。
- `set_homecmd()`: 机械臂执行回零动作。

### 末端工具 (End Effector)
- `set_endeffector_suctioncup(enable, on)`: 控制吸嘴。`enable` 开启，`on` 吸取。
- `set_endeffector_gripper(enable, on)`: 控制夹爪。`enable` 开启，`on` 闭合。

---

## 4. 视觉与复合动作 (`beta_go`)

`beta_go` 提供了视觉算法转换及部分场景化的宏函数。

### 视觉检测与转换
- `set_arm_camera_model(index)`: 设置机械臂摄像头识别模型（1: 积木, 2: AprilTag, 3: 生鲜/快递）。
- `set_car_camera_model(index)`: 设置小车摄像头识别模型（如路标等）。
- `get_arm_camera_model()` / `get_car_camera_model()`: 获取当前生效的摄像头模型。
- `creat_apriltag_obj(id, height)`: 创建并注册用户自定义的 AprilTag 物体高度参数。
- `get_apriltag_obj_height(id)` / `get_apriltag_obj_z(id)`: 获取已创建的 AprilTag 物体高度及吸附点 Z 轴坐标参数。
- `imgxy_to_armxy(px, py, need_tranxy)`: 将图像坐标 `(px, py)` 转换为机械臂空间坐标。
- `arm_camera_is_detected(obj_name)`: 是否检测到指定名称的物体。
- `car_camera_is_detected(sign_name)`: 小车摄像头是否检测到指定路标（如 `"stop"`, `"l"`, `"r"`）。

### 复合动作 (Compound Actions)
- `into_park_space(garage_class)`: 自动入库。`0` 仓库，`1` 超市。
- `out_park_space(garage_class)`: 自动出库。
- `grab_obj_floortocar(object_class)`: 将地面物品抓取到小车。
- `grab_obj_cartofloor(object_class)`: 将小车物品卸载到地面。
- `set_ptp_car()`: 将机械臂移动到小车上方拍照位。
- `set_ptp_floor()`: 将机械臂移动到地面上方拍照位。

---

## 5. 基础外设工具 (`util`)

`util` 对象用于获取外部硬件数据传入 AI 服务器。
- `get_image(timeout, port, flip, name, width, height)`: 激活并自动获取 PC 摄像头画面 / 拍照返回给图像识别接口。
- `record(timeout)`: 使用 PC 麦克风录制一段语音，返回的音频数据可用于 `speech.asr()`。

---

## 6. AI 服务 (OCR/Face/Speech)

> [!NOTE]
> AI 服务接口需要通过 `DobotEDU(account, password)` 正确初始化有效的 Token 并确保联网环境。由于底层对接云端服务，这些方法可能存在通信延迟。

- `face`: 人脸检测与对比、创建人脸库与检索。
- `ocr`: 提取图像中的文本（基础通用字符或身份证）。
- `speech`: 语音识别 (ASR) 与在线语音合成。
- `nlp`: 自然语言处理逻辑（如文章主题词提取）。
- `tmt`: 机器翻译，例如 `tmt.translation(source_text, source, target)`。
- `robot`: AI 机器人闲聊服务 (`robot.conversation`)。
- `ai (pyimageom)`: 特征图像提取切图、云端特征及分类器。

---

## 常用常量参考

### 机械臂 PTP 模式
- `0`: JUMP (门形运动)
- `1`: MOVJ (关节运动)
- `2`: MOVL (直线运动)

### 小车摄像头路标 ID
`"lors"`, `"l"`, `"p"`, `"apt"`, `"rors"`, `"r"`, `"stop"`, `"spm"`, `"t"`, `"u"`, `"wh"`, `"z"`
