# 6.22.1 SetLanPortConfig

KeyWords:

portName: string

addr: string

mask: string

gateway: string

dns: string

isdhcp: bool



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.M1.SetLanPortConfig",
    "params": {
        "portName": "COM4",
        "addr": "192.168.2.87",
        "mask": "255.255.255.0",
        "gateway": "192.168.2.1",
        "dns": "0.0.0.0",
        "isdhcp": true
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.) This file is decompiled from a .CHM file  by an UNREGISTERED version of Easy CHM.  You can download Easy CHM at :  http://www.eTextWizard.com