### 8.15.1 AuxSetSwitch

**Description: 设置扩展轴开关**

**KeyWords:**

portName: string

auxJoint: bool，轴功能开关

addPoints: bool，示教点功能开关

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.AuxSetSwitch",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "auxJoint": true,
            "addPoints": true
        }
    }
}
```
