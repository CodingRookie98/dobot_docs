# Python 程序集成与应用示例

## Python Program Demo

Demo 1: 控制机器人绘制一个正方形

```python
#落笔点的位置
from DobotEDU import *
x = 250
y = 0
z = -47
#控制机器人末端门型运动至落笔点处
m_lite.set_ptpcmd(0, x, y, z, 0)
side = 30  #正方形的边长
m_lite.set_ptpcmd(1, x+side, y, z, 0)
m_lite.set_ptpcmd(1, x+side, y-side, z, 0)
m_lite.set_ptpcmd(1, x, y-side, z, 0)
m_lite.set_ptpcmd(1, x, y, z, 0)

```

Demo 2：控制机器人将积木从A点（257, -143, -38）运送至B点（272, 57, -38）

```python
#机器人初始化设置
from DobotEDU import *
m_lite.set_ptpcmd(0, 250, 0, 50, 0)  #机器人初始位置

m_lite.set_ptpcmd(0, 257, -143, -38, 0)  #机器人运动到A区
m_lite.set_endeffector_suctioncup(True, True)  #吸盘吸取积木
m_lite.set_ptpcmd(0, 272, 57, -38, 0)  #机器人运动到B区
m_lite.set_endeffector_suctioncup(True, False)  #吸盘释放积木
m_lite.set_ptpcmd(0, 250, 0, 50, 0)  #机器人回到初始位置
m_lite.set_endeffector_suctioncup(False, False)  #关闭吸盘

```

---

## 附录

### Dobot 硬件设备使用手册下载：

**Dobot Magician / Magician Lite / Magician Go**

您可前往越疆 资料下载中心 获取相关硬件设备的最新使用手册。

---
