# 4.2.3 SetDeviceName

Set device name



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |
| deviceName | string | yes | device name to be  
set |




response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result（true：set succeeded，false：set 
  failed） |






KeyWords:

portName: string

deviceName: string

INPUT

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "method": "dobotlink.MagicianLite.SetDeviceName",    "params": {        "portName": "COM15",        "deviceName": "Dobot123"   }
}
```



OUTPUT:

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true} 

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com