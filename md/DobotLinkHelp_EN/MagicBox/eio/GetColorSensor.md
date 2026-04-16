# 5.7.12 GetColorSensor

Get color sensor



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |





response result


| field | type | required | explain |
| --- | --- | --- | --- |
| blue | int | yes | blue threshold |
| green | int | yes | green threshold |
| red | int | yes | red 
threshold |





KeyWords:

portName: string

red: int

green: int

blue: int



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.GetColorSensor",
    "params": {
        "portName": "COM4"
    }
}
```





OUTPUT:

```json

```json

{
    "id": 1,    "jsonrpc": "2.0",    "result": {
        "blue": 0,        "green": 0,        "red": 0
    }
}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com