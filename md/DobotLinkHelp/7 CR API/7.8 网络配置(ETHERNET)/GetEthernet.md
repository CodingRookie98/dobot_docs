### 7.8.2 GetEthernet

**KeyWords:**

portName: string

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.GetEthernet",
    "params": {
        "portName": "192.168.5.1"
    }
}
```

OUTPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "dhcp": false,
        "ip": "192.168.5.105",
        "netmask": "255.255.255.0",
        "gateway": "192.168.0.1"
    }
}
```
