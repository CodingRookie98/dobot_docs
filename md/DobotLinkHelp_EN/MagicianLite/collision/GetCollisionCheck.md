# 4.12.2 GetCollisionCheck

Read collision detection function




request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




response result

| field | type | required | explain |
| --- | --- | --- | --- |
| isEnabled | bool | yes | enable collision function (false: No, true: 
      Yes) |
| threshold | float | yes | angle threshold triggered by collision 
      detection, in ° |







KeyWords:

portName: string

isEnabled: bool

threshold: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetCollisionCheck",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "isEnabled": true,        "threshold": 8    }    
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com