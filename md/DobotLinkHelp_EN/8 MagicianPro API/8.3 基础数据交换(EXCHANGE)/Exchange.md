**KeyWords:**

portName: string

data: object

 

INPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "method": "dobotlink.MagicianPro.Exchange",
    "params": {
        "portName": "192.168.1.6",
        "data": {
            "controlMode": "enable",
            "coordinate": "joint",
            "hardware": true,
            "jogMode": "jog",
            "alarms": false,
            "outputs": {
                "enable": false,
                "value": [0, 0, 0, 0, 0, 0, 0, 0]
            },
            "toolCoordinate": 0,
            "userCoordinate": 0
        }
    }
}
```

 

OUTPUT:

``` language-json
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": {
        "alarms": [null, [],
            [],
            [],
            []
        ],
        "armOrientation": 1,
        "autoManual": "manual",
        "cartesianCoordinate": [400, 0, 0, 0],
        "controlMode": "disable",
        "coordinate": "joint",
        "inputs": [0, 0, 0, 0, 0, 0, 0, 0],
        "jogMode": "jog",
        "jointCoordinate": [0, 0, 0, 0],
        "outputs": [0, 0, 0, 0, 0, 0, 0, 0],
        "toolCoordinate": 0,
        "userCoordinate": 0
    }
}
```