### 8.3.21 SetExtendIO

**Description: 设置扩展IO**

**KeyWords:**

portName: string

data: object

INPUT:

```json
{
"id": 1,
"jsonrpc": "2.0",
"method": "dobotlink.MagicianPro.SetExtendIO",
"params": {
"portName": "192.168.9.1",
"data": {
"enable": true,
"extendDO": {
"enable": true,
"value": [
[11, 45, 36, 30, 11, 45, 127, 255, 0, 0, 0, 0]
]
}
}
}
}
```
<div>

</div>

<div>

</div>

<div>

OUTPUT:

</div>

<div>

```json
{
"id": 1,
"jsonrpc": "2.0",
"result": {
"value": true
}
}
```

</div>
