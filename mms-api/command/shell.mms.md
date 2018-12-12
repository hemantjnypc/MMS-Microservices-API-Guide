---
description: Bash emulation
---

# shell.mms

|  | Description |
| :--- | :--- |
| cmd | Copy, Delete, List, Make Directory, Execution, Find |

shell@hello.ypcloud.com

| Function | Parameters | Return |
| :--- | :--- | :--- |
| **Cmd\(\)** | {"cmd":"cp","options":"STRING","source":"STRING","dest":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"cp","options":"-f","source":"321.jpg ","dest":"556.jpg "} | {"Result":"OK"} |
| cp | {"cmd":"cp","source":"STRING","dest":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"cp","source":"321.jpg","dest":"556.jpg"} | {"Result":"OK"} |
| **Cmd\(\)** | {"cmd":"rm","options":"STRING","file":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"rm","options":"-f","file":"123.jpg"} | {"Result":"OK"} |
| rm | {"cmd":"rm","file":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"rm","file":"123.jpg"} | {"Result":"OK"} |
| **Cmd\(\)** | {"cmd":"ls","options":"STRING","path":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"ls","options":"STRING","path":"D:\nodejs\project"} | {"Result":\["HelloWorld","Bin","comm"\]} |
| Is | {"cmd":"ls","path":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"ls","path":"D:\nodejs\project"} | {"Result":\["HelloWorld","Bin","comm"\]} |
| **Cmd\(\)** | {"cmd":"mkdir","options":"STRING","dir":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"mkdir","options":"-p","dir":"test"} | {"Result":"OK"} |
| mkdir | {"cmd":"mkdir","dir":"STRING"} | {"Result":"STRING"} |
|  | {"cmd":"mkdir","dir":" test "} | {"Result":"OK"} |
| **Cmd\(\)** | {"cmd":"exec","command":"String"} | {"Result":"STRING"} |
| exec | {"cmd":"exec","command":"node HelloWorld"} | {"Result":"OK"} |
| **Cmd\(\)** | {"cmd":"find"," path ":"STRING"} | {"Result":"STRING"} |
| find | {"cmd":"find"," path ":"HelloWorld"} | {"Result":" HelloWorld "} |

Reference : [https://www.npmjs.com/package/shelljs](https://www.npmjs.com/package/shelljs)

