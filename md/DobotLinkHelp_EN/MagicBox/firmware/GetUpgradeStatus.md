# 5.9.2 GetUpgradeStatus

Get firmware burning status 



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| length | string | yes | firmware length |
| md5 | string | yes | MD5 check 
code |


response result
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |




Description: switch the device to firmware burning mode

KeyWords:

portName: string

length: string

md5: string

latest: bool



INPUT:



```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetUpgradeStatus",
    "params": {
        "portName": "COM4",
        "length": "B0060800",
        "md5": "6094308AA9DED6A612A620AC4A195615"
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com