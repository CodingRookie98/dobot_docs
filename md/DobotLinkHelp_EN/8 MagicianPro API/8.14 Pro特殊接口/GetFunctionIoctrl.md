**Description: 远程IO配置**

**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.GetFunctionIoctrl",
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
         "in":{
        "clear_alarm":11,
         "continue":12, 
         "pause_pin":13, 
         "stop_pin":14, 
         "start_pin":15,
         "emergencystop":16
    },
    "out":{
        "readystatus":13, 
        "pausestatus":14, 
        "alarmstatus":15, 
        "runstatus":16
    }
    }
}
```