# 4.12.1 SetCollisionCheck

Set collision detection function



request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| enable | bool | yes | enable collision function (false: No, true: 
  Yes) |
| threshold | float | yes | angle threshold triggered by collision detection, in ° (value 
      range: 8-15) |




response result


| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |









KeyWords:

portName: string

enable: bool

threshold: float (min:8 unit:angle)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.SetCollisionCheck",
    "params": {
        "portName": "COM4",
        "enable": true,
        "threshold": 9.5
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com