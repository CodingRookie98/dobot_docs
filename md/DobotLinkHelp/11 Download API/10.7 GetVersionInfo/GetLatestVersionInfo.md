## 10.7 GetVersionInfo

**KeyWords:**

device: string

version: string, 版本号，

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.GetVersionInfo",
    "params": {
        "device": "MagicBox",
        "version": "1.0.6.6"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
              "info": "2020/08/29 Ver1.0.6.6rn1、增加Blockly中获取时间指令接口；rn2、增加Blockly末端坐标偏移量指令；rn3、修复末端类型指令离线指令；rn4、修复离线滑轨回零无法停止问题；rn5、增加滑轨/传送带复位时停止的功能；rn6、修复Blockly获取角度/坐标指令报错问题；rn7、修复Blockly吸盘手爪运行报错问题；rn8、增加设置滑轨速度同步指令。rn"
    }
}
```
