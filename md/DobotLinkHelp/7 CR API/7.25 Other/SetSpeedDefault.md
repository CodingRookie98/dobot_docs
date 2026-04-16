INPUT:

```json
{
"id":1,
"jsonrpc":"2.0",
"method":"dobotlink.CR.SetSpeedDefault",
"params":{
"portName":"192.168.5.1",
"data":{"common":{"ratio":{"def":50,"max":100,"min":1}},"dragSensivity":{"j1":{"def":50,"max":90,"min":1},"j2":{"def":50,"max":90,"min":1},"j3":{"def":50,"max":90,"min":1},"j4":{"def":50,"max":90,"min":1},"j5":{"def":50,"max":90,"min":1},"j6":{"def":50,"max":90,"min":1}},"playback":{"arch":{"endHeight":{"def":20,"max":1300,"min":1},"startHeight":{"def":20,"max":1300,"min":1},"zLimit":{"def":50,"max":1300,"min":1}},"coordinate":{"acceleration":[{"def":10000,"max":999999,"min":1},{"def":10000,"max":999999,"min":1},{"def":10000,"max":999999,"min":1},{"def":900,"max":999999,"min":1},{"def":900,"max":999999,"min":1},{"def":900,"max":999999,"min":1}],"jerk":[{"def":18000,"max":999999,"min":1},{"def":18000,"max":999999,"min":1},{"def":18000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1},{"def":9000,"max":999999,"min":1}],"velocity":[{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1}]},"joint":{"acceleration":[{"def":200,"max":999999,"min":1},{"def":200,"max":999999,"min":1},{"def":200,"max":999999,"min":1},{"def":500,"max":999999,"min":1},{"def":500,"max":999999,"min":1},{"def":500,"max":999999,"min":1}],"jerk":[{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":2000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1},{"def":5000,"max":999999,"min":1}],"velocity":[{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1},{"def":180,"max":999999,"min":1}]}},"teach":{"coordinate":{"acceleration":[{"def":300,"max":999999,"min":1},{"def":300,"max":999999,"min":1},{"def":300,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1}],"velocity":[{"def":50,"max":999999,"min":1},{"def":50,"max":999999,"min":1},{"def":50,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1}]},"joint":{"acceleration":[{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1},{"def":100,"max":999999,"min":1}],"velocity":[{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1},{"def":12,"max":999999,"min":1}]}}}
}
}
```
:::

OUTPUT：

```json
{
 "id": 1,
 "jsonrpc": "2.0",
 "result": true
}
```
Copyright © 2019. All rights reserved. (To change the copyright info,
just edit it in template.)
