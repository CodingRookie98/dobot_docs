**KeyWords:**

portName: string

value: array

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetExtendDO",
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
  "value": [
   [1, 11, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
  ]
 }
}
```