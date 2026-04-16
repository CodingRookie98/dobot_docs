### 6.22.2 GetLanPortConfig

**KeyWords:**

portName: string

isConnected: bool

addr: string

mask: string

gateway: string

dns: string

isdhcp: bool

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.GetLanPortConfig",
    "params": {
        "portName": "COM4"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "isConnected": true,
        "addr": "192.168.2.87",
        "mask": "255.255.255.0",
        "gateway": "192.168.2.1",
        "dns": "0.0.0.0",
        "isdhcp": true
    }
}
```
