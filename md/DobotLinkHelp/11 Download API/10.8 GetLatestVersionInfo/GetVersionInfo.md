## 10.8 GetLatestVersionInfo

**Description: 获取最新的固件信息**

**KeyWords:**

device: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.Download.GetLatestVersionInfo",
    "params": {
        "device": "Magician"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
             "info": "2020/03/23 Ver2.0.7.0版本  CJTrn1，修复GD USB长时间工作挂掉的问题,rn2，增加对gd外部flash的支持rn3，开启规划算法精度修复的宏rn4，修复点动运动触发报警后，点动速度未置0导致发送停止点动指令会运动一段距离的问题rn"
   }
}
```
