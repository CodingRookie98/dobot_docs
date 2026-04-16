# 4.8.8 GetEndEffectorGripper

Get claw output

reuqest params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |






response result

| field | type | required | explain |
| --- | --- | --- | --- |
| isEnabled | bool | yes | Control whether it is enabled (true: Yes, 
      false: no) |
| isOn | bool | yes | Whether the claw is caught (true: Yes, 
      false: no) |







KeyWords:

portName: string

isEnabled: bool

isOn: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorGripper",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT：

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "isEnabled": false,        "isOn": false    }}


```json

```

Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com