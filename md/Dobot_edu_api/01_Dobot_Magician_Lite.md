# Dobot Magician Lite 机械臂控制指令

## 3.1 Dobot Magician Lite

---

## 运动

---

## 执行点到点指令

-
原型：

```python
m_lite.set_ptpcmd(ptp_mode,x,y,z,r)

```

-
描述：从当前位置运动至目标位置。

-
必选参数：

  - x：X轴坐标，数据类型：float。

  - y：Y轴坐标，数据类型：float。

  - z：Z轴坐标，数据类型：float。

  - r：R轴坐标，数据类型：float。

  - ptp_mode：PTP 模式，数据类型：int，取值范围：0 ~ 9。

    - 0：JUMP 模式，(x, y, z, r)为笛卡尔坐标系下的目标点坐标。

    - 1：MOVJ 模式，(x, y, z, r)为笛卡尔坐标系下的目标点坐标。

    - 2：MOVL 模式，(x, y, z, r)为笛卡尔坐标系下的目标点坐标。

    - 3：JUMP 模式，(x, y, z, r)为关节坐标系下的目标点坐标。

    - 4：MOVJ 模式，(x, y, z, r)为关节坐标系下的目标点坐标。

    - 5：MOVL 模式，(x, y, z, r)为关节坐标系下的目标点坐标。

    - 6：MOVJ 模式，(x, y, z, r)为关节坐标系下的坐标增量。

    - 7：MOVL 模式，(x, y, z, r)为笛卡尔坐标系下的坐标增量。

    - 8：MOVJ 模式，(x, y, z, r)为笛卡尔坐标系下的坐标增量。

    - 9：JUMP 模式，平移时运动模式为 MOVL，(x, y, z, r)为笛卡尔坐标系下的坐标增量。

-
返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
m_lite.set_ptpcmd(ptp_mode=0, x=200, y=20, z=10, r=0)

```

以JUMP 模式，使机械臂从当前位置运动至目标位置(200, 20, 10, 0)。

---

## 执行回零指令

-
原型：

```python
m_lite.set_homecmd()

```

-
描述：机械臂从当前位置运行至零点位置。

-
必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_homecmd()

```

机械臂从当前位置运行至零点位置。

---

## 设置吸盘状态

-
原型：

```python
m_lite.set_endeffector_suctioncup(enable, on)

```

-
描述：设置末端吸盘的状态。

-
必选参数：

  - enable：吸盘是否使能。True：吸盘使能；False：吸盘未使能。

  - on：吸盘吸取或释放。True：吸盘吸取；False：吸盘释放。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_endeffector_suctioncup(enable=True, on=True)

```

末端吸盘上使能，并且吸盘为吸取状态。

---

## 设置夹爪状态

-
原型：

```python
m_lite.set_endeffector_gripper(enable, on)

```

-
描述：设置末端夹爪的状态。

-
必选参数：

  - enable：夹爪是否使能。True：夹爪使能；False：夹爪未使能。

  - on：夹爪抓取或释放。True：夹爪抓取；False：夹爪释放。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_endeffector_gripper(enable=True, on=True)

```

末端夹爪上使能，并且夹爪为抓取状态。

---

## 检测

---

## 获取末端类型

-
原型：

```python
m_lite.get_end_effector_type()

```

-
描述：获取末端的类型。

-
必选参数：无

- 返回：

  - type：末端类型。0：无末端；1：末端为吸盘；2：末端为夹爪；3：末端为笔。

-
示例

```python
type = m_lite.get_end_effector_type()
print(type)

```

获取末端的类型。

---

## 获取机械臂实时位姿

-
原型：

```python
m_lite.get_pose()

```

-
描述：获取机械臂的实时位姿。

-
必选参数：无

-
返回：{x, y, z, r, jointAngle }

  - x：X 轴坐标。

  - y：X 轴坐标。

  - z：Z 轴坐标。

  - r：R 轴坐标。

  - jointAngle：关节坐标列表 [关节 1,关节 2,关节 3,关节 4]。

-
示例

```python
result = m_lite.get_pose()
print(result)

```

获取机械臂的实时位姿。

---

## 获取机械臂速度比例

-
原型：

```python
m_lite.get_armspeed_ratio(get_type)

```

-
描述：获取机械臂不同运动模式的运动速度比例。

-
必选参数：

  - get_type：运动模式。0：点动。 1：点到点运动。

- 返回：

  - ratio：运动模式对应的运动速度比例。

-
示例

```python
result = m_lite.get_armspeed_ratio(get_type=1)
print(result)

```

获取机械臂的点到点运动模式对应的运动速度比例。

---

## 检测丢步结果

-
原型：

```python
m_lite.get_lost_step_result()

```

-
描述：检测丢步结果。

-
必选参数：无

- 返回：

  - state：系统报警状态。

-
示例

```python
result = m_lite.get_lost_step_result()
print(result)

```

检测丢步结果。

---

## 设置

---

## 设置丢步阈值

-
原型：

```python
m_lite.set_lost_step_params(value)

```

-
描述：设置丢步检测阈值，用于检测定位误差是否超过该阈值。如果超过该阈值， 则说明电机丢步。

-
必选参数：

  - value：丢步阈值。数据类型：int。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_lost_step_params(value=10)

```

设置丢步检测阈值为10。

---

## 设置机械臂速度比例

-
原型：

```python
m_lite.set_armspeed_ratio(set_type, set_value)

```

-
描述：设置机械臂不同运动模式的运动速度比例。

-
必选参数：

  - set_type：运动模式。 0：点动。 1：点到点运动。 2：连续轨迹运动。 3：圆弧运动。

  - set_value：运动模式对应的运动速度比例，数据类型：int，取值范围：0 ~ 100。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_armspeed_ratio(set_type=1, set_value=50)

```

设置机械臂的点到点运动模式对应的运动速度比例为50%。

---

## 设置门型运动参数

-
原型：

```python
m_lite.set_ptpjump_params(z_limit, jump_height)

```

-
描述：设置门型运动的参数。

-
必选参数：

  - z_limit：最大抬升高度。 数据类型：int。

  - jump_height：抬升高度。数据类型：int。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

- 示例
```python
m_lite.set_ptpjump_params(z_limit=100, jump_height=100)

```

设置门型运动时，最大抬升高度为100，抬升高度为100。

---

## 等待 n 秒

-
原型：

```python
m_lite.wait(delay)

```

-
描述：设置等待时间。

-
必选参数：

  - delay：等待时间。数据类型：int，单位：s。

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.wait(delay=10)

```

设置等待时间为10 s。

---

## 执行检测丢步

-
原型：

```python
m_lite.set_lost_step_cmd()

```

-
描述：丢步检测。

-
必选参数：无

- 返回：

  - True： 指令完成。

  - False： 指令未完成。

-
示例

```python
m_lite.set_lost_step_cmd()

```

执行丢步检测。

---
