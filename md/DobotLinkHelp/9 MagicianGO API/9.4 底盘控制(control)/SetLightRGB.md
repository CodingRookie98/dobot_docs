### 9.4.14 SetLightRGB

**KeyWords:**

portName: string

number: int
(RGB灯的使能状态（从低位到高位依次表示对应序号灯的使能状态，用户灯：0x0FC3）)

effect: int
(0：常亮模式，1：定时熄灭，2：呼吸模式，3：闪烁模式，4：彩虹呼吸渐变模式，5：流水环绕，0xFF，跟随状态灯
)

r: int (红色亮度值（0-255）)

g: int (绿色亮度值（0-255）)

b: int (蓝色亮度值（0-255）)

cycle: float （周期（单位s）（如果是定时熄灭模式代表亮的时间,单位s））

counts: int （次数：闪烁烁模式有效 -1：无限次， 1：1次，2：2次... ）

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianGO.SetLightRGB",
    "params": {
        "portName": "COM4",
        "number": 0,
        "effect": 0,
        "r": 0,
        "g": 0,
        "b": 0,
        "cycle": 1.0,
        "counts": 1
    }
}
```
