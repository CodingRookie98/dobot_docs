# 4.8.4 GetEndEffectorType

Get end fitting type


request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
device |



reponse result
| field | type | required | explain |
| --- | --- | --- | --- |
| type | int | yes | reponse result |






KeyWords:

portName: string

type: int (0:None 1:SucktionCup 2:Gripper 3:Pen)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetEndEffectorType",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "type": 1    }}



```

Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com