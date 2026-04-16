### 4.1.1 SearchDobot

<div>

**查看设备的当前状态**

</div>

<div>

</div>

<div>

请求参数 params

</div>

<div>

</div>

<div>

</div>

<div>

</div>

<div>

  ----------- ----------- ------------ -------------------------------
  字段      类型      是否必填   说明
  portName   string   是          设备的通信端口
  filter     string    是          过滤连接方式（如串口的名称）
  ----------- ----------- ------------ -------------------------------

</div>

<div>

</div>

<div>

响应参数 result

</div>

<div>

  -------------- ---------- ------------ ----------------------
  字段          类型     是否必填   说明
  portName      string   是          设备的通信端口
  status        string   是         设备的当前状态（connected：已连接，unconnected：未连接，occupied：被占用，unknown：未知的）
  description   string   是         设备描述
  -------------- ---------- ------------ ----------------------
</div>

<div>

</div>

**KeyWords:**

portName: string

status: string (connected, unconnected, occupied, unknown)

filter: string (separate with ' ')

请求:

<div>

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SearchDobot",
    "params": {
        "filter": "Bluetooth VM-3..."
    }
}
```

</div>

响应:

<div>

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": [{
        "portName": "COM3",
        "status": "unconnected",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }, {
        "portName": "COM15",
        "status": "occupied",
        "description": "Silicon Labs CP210x USB to UART Bridge"
    }]
}
```

</div>
