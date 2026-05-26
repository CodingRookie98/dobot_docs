**KeyWords:**

portName: string

data: object

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetEthernet",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "dhcp": false,
            "ip": "192.168.5.105",
            "netmask": "255.255.255.0",
            "gateway": "192.168.0.1"
        }
    }
}
```
