**功能: 获取拖拽示教点列表**

 

INPUT:

``` language-json
{    

    "id": 1,    

    "jsonrpc": "2.0",    

    "method": "dobotlink.CR.GetDragTeachFileList",

    "params": {       
        "portName": "192.168.1.6"
    }

}
```

 

OUTPUT:

``` language-json
{
   "id": 1,
    "jsonrpc": "2.0",
    "result": 
[
  "/project/xxx/xxx/111.json", 

  "/project/xxx/xxx/222.json", 

  "/project/xxx/xxx/333.json"
 ]
}
```