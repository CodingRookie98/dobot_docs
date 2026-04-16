# 8.2.4 WriteFile

KeyWords:

portName: string

fileName: string

content: object/string

url: string (if url is null, it will not send post request)



INPUT:

```json

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.WriteFile",
    "params": {
        "portName": "192.168.1.6",
        "fileName": "/xxx/xxx.json",
        "content": {
            ...
        },
        "url": "/xxx/xxx"
    }
}
```
Copyright © 2019. All rights reserved. (To change the copyright info, just edit it in template.)