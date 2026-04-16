## 2.5 ShowAvailablePorts

**Description: 返回当前电脑所有串口**

**KeyWords:**

portName: string

description: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.api.ShowAvailablePorts"
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [{
        "portName": "COM3",
        "description": "Arduino Uno"
    }, {
        "portName": "COM4",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }]
}
```
