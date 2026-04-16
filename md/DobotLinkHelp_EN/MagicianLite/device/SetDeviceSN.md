# 4.2.1 SetDeviceSN

Set device serial number



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| deviceSN | string | yes | serial number to be set (starting with 
DT14) |






response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result（true：operation succeeded，false：operation 
  failed） |


KeyWords:

portName: string

deviceSN: string (start with 'DT14')



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetDeviceSN",
    "params": {
        "portName": "COM4",
        "deviceSN": "DT1418080700"
    }
}
```



OUTPUT:



```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}  

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com