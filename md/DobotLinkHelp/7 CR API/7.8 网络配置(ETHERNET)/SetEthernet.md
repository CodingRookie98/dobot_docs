### 7.8.1 SetEthernet

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.SetEthernet",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "dhcp": false,
            "ip": "192.168.5.105",
            "netmask": "255.255.255.0",
            "gateway": "192.168.0.1"
        }
    }
}
```
