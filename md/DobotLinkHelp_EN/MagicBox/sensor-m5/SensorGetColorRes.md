# 12.1.22 SensorGetColorRes

Read color recognition results



Note: before using this interface, you need to use the SensorColorInit interface



request params




| field | type | required | explain |
| --- | --- | --- | --- |
| portName | string | yes | communication port of the device |
| port | int | yes | communication port 
(0~5) |





response result

| field | type | required | explain |
| --- | --- | --- | --- |
| color | string | yes | color recognition 
      results(none/red/green/blue/yellow) |






KeyWords:

portName: string

port: int (0~5)

color: string (none/red/green/blue/yellow)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicBox.SensorGetColorRes",
    "params": {
        "portName": "COM4",
        "port": 2
    }
}
```

OUTPUT：

```json

```json

{    "id": 1,    "jsonrpc": "2.0",    "result": {        "color": "black"    }
}

 

```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com