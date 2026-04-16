# 12.1.31 SensorSetSYNCmd

Voice module control command



request params


| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port（1） |
| cmd | int | yes | voice command(0: stop playing, 1: pause 
      playing, 2: continue playing, 3: next song, 4: previous 
      song) |







response result



| field | type | required | explain |
| --- | --- | --- | --- |
| result | bool | yes | response result (true: operation succeeded, 
      false: operation failed) |






KeyWords:

portName: string

port: int (1)

cmd: int (0:stop 1:suspend 2:resume 3:next 4:previous)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorSetSYNCmd",
    "params": {
        "portName": "COM4",
        "port": 1,
        "cmd": 0
    }
}
```

OUTPUT：

```json

```json
{    "id": 1,    "jsonrpc": "2.0",    "result": true}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com