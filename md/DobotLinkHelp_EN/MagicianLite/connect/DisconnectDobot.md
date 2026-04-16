# 4.1.3 DisconnectDobot

Disconnect the device


request params
| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| queueStop | bool | yes | stop the 
      queue, the default 
      is true(true：start stop queue operation，false：close stop queue 
      operation) |
| queueClear | bool | yes | clear 
      queue,  the default 
      is true(true：open clear queue operation，false：close clear queue 
      operation) |

response result 
| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | connection status of the device（true：connection succeeded，false：connection 
      failed） |




KeyWords:

portName: string

*queueStop: bool (default:true)

*queueClear: bool (default:true)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianLite.DisconnectDobot",
    "params": {
        "portName": "COM4",
        "queueStop": true,
        "queueClear": true
    }
}
```


OUTPUT：
```json

```json
     
{    "id": 56,    "jsonrpc": "2.0",    "result": true}

```




Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com