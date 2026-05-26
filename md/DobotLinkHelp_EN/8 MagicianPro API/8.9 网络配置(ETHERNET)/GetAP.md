**KeyWords:**

portName : string

ssid : string

passwd : string

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetAP",
    "params": {
        "portName": "192.168.1.6"
    }
}
```

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "ssid": "dobot",
        "passwd": "bingezuishuai"
    }
}
```
