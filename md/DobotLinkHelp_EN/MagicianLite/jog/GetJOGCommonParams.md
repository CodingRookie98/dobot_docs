# 4.9.6 GetJOGCommonParams

Get jog common parameters


 request params



| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the 
  device |




response result

| field | type | required | explain |
| --- | --- | --- | --- |
| accelerationRatio | float | yes | s |
| velocityRatio | float | yes | a |











KeyWords:

portName: string

velocityRatio: float

accelerationRatio: float



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.GetJOGCommonParams",
    "params": {
        "portName": "COM4"
    }
}
```



OUTPUT:



```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "accelerationRatio": 50,        "velocityRatio": 100    }}


```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com