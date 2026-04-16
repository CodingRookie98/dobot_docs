### 7.2.4 WriteFile

**KeyWords:**

portName: string

fileName: string

content: object/string

url: string (if url is null, it will not send post request)

INPUT:

```json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.CR.WriteFile",
    "params": {
        "portName": "192.168.5.1",
        "fileName": "/xxx/xxx.json",
        "content": {
            ...
        },
        "url": "/xxx/xxx"
    }
}
```
