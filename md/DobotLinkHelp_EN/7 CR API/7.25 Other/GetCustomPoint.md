功能:

获取初始姿态  

 

INPUT:

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0",

    "method": "dobotlink.CR.GetCustomPoint",

    "params": {

        "portName": "192.168.5.1"

     }


  }


 
```

OUTPUT：

``` language-json
{

    "id": 1,

    "jsonrpc": "2.0", 

     "result": {"joint":[0.0,0.0,0.0,0.0,0.0,0.0]}


  }
```