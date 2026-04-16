# 4.10.8 GetPTPJumpParams

Obtain door mode point parameters

request params

| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |






response result

| field | type | required | explain |
| --- | --- | --- | --- |
| jumpHeight | float | yes | lifting distance of door mode movement |
| zLimit | float | yes | maximum lifting height limit of door mode 
      movement |





KeyWords:

portName: string

zLimit: float

jumpHeight: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetPTPJumpParams",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": {        "jumpHeight": 20,        "zLimit": 100    }    
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com