# 5.2.1 SetDeviceSN

Device information setting device serial number



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| deviceSN | string | yes | serial number to be set (starting with 
DT14) |






 response result
| field | type | required | explain |
| --- | --- | --- | --- |
| deviceSN | string | yes | device serial number |




KeyWords:

portName: string

deviceSN: string (start with 'DT14')



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SetDeviceSN",
    "params": {
        "portName": "COM4",
        "deviceSN": "DT1418080700"
    }
}
```



 OUTPUT:



```json
 {     "id": 1,     "jsonrpc": "2.0",     "result": {         "deviceSN": "\u0002"     } }
```

```json

    
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com