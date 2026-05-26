**Description: 自动/手动**

**KeyWords:**

portName: string

data: object

value: string

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.SetAutoManualMode",
    "params": {
        "portName": "192.168.5.1",
        "data": {
            "value": "auto"/"manual"
        }    
    }
}
```