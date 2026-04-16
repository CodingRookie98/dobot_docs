# 4.2.5 GetDeviceID

Get device ID



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| deviceID | array(int) | yes | device ID 
data |






KeyWords:

portName: string

deviceID: array (int)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetDeviceID",
    "params": {
        "portName": "COM15"
    }
}
```



OUTPUT:

```json

```json


{    "id": 1,    "jsonrpc": "2.0",    "result": {        "deviceID": [48, 255, 218]    }}

```

Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com